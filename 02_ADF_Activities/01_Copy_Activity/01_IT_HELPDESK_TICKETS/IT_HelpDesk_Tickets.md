{
    "name": "Pl_Helpdesk",
    "properties": {
        "activities": [
            {
                "name": "Get Metadata1",
                "type": "GetMetadata",
                "dependsOn": [],
                "policy": {
                    "timeout": "0.12:00:00",
                    "retry": 0,
                    "retryIntervalInSeconds": 30,
                    "secureOutput": false,
                    "secureInput": false
                },
                "userProperties": [],
                "typeProperties": {
                    "dataset": {
                        "referenceName": "Json2",
                        "type": "DatasetReference"
                    },
                    "fieldList": [
                        "childItems"
                    ],
                    "storeSettings": {
                        "type": "AzureBlobStorageReadSettings",
                        "recursive": true,
                        "enablePartitionDiscovery": false
                    },
                    "formatSettings": {
                        "type": "JsonReadSettings"
                    }
                }
            },
            {
                "name": "Filter1",
                "type": "Filter",
                "dependsOn": [
                    {
                        "activity": "Get Metadata1",
                        "dependencyConditions": [
                            "Completed"
                        ]
                    }
                ],
                "userProperties": [],
                "typeProperties": {
                    "items": {
                        "value": "@activity('Get Metadata1').output.childItems",
                        "type": "Expression"
                    },
                    "condition": {
                        "value": "@contains(item().name,'.json')",
                        "type": "Expression"
                    }
                }
            },
            {
                "name": "ForEach1",
                "type": "ForEach",
                "dependsOn": [
                    {
                        "activity": "Filter1",
                        "dependencyConditions": [
                            "Completed"
                        ]
                    }
                ],
                "userProperties": [],
                "typeProperties": {
                    "items": {
                        "value": "@activity('Filter1').output.value",
                        "type": "Expression"
                    },
                    "isSequential": true,
                    "activities": [
                        {
                            "name": "Copy data1",
                            "type": "Copy",
                            "dependsOn": [],
                            "policy": {
                                "timeout": "0.12:00:00",
                                "retry": 0,
                                "retryIntervalInSeconds": 30,
                                "secureOutput": false,
                                "secureInput": false
                            },
                            "userProperties": [],
                            "typeProperties": {
                                "source": {
                                    "type": "JsonSource",
                                    "storeSettings": {
                                        "type": "AzureBlobStorageReadSettings",
                                        "recursive": true,
                                        "wildcardFileName": "*.json",
                                        "enablePartitionDiscovery": false
                                    },
                                    "formatSettings": {
                                        "type": "JsonReadSettings"
                                    }
                                },
                                "sink": {
                                    "type": "JsonSink",
                                    "storeSettings": {
                                        "type": "AzureBlobStorageWriteSettings"
                                    },
                                    "formatSettings": {
                                        "type": "JsonWriteSettings"
                                    }
                                },
                                "enableStaging": false
                            },
                            "inputs": [
                                {
                                    "referenceName": "Json3",
                                    "type": "DatasetReference",
                                    "parameters": {
                                        "FileName": {
                                            "value": "@item().name",
                                            "type": "Expression"
                                        }
                                    }
                                }
                            ],
                            "outputs": [
                                {
                                    "referenceName": "Json4",
                                    "type": "DatasetReference",
                                    "parameters": {
                                        "FileName": {
                                            "value": "@item().name",
                                            "type": "Expression"
                                        }
                                    }
                                }
                            ]
                        }
                    ]
                }
            }
        ],
        "parameters": {
            "FileName": {
                "type": "String"
            }
        },
        "annotations": []
    }
}