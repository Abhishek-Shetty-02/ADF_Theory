**Pl\_webactivity resource in json:**



{

&nbsp;   "name": "Pl\_webactivity",

&nbsp;   "properties": {

&nbsp;       "activities": \[

&nbsp;           {

&nbsp;               "name": "Web1",

&nbsp;               "type": "WebActivity",

&nbsp;               "dependsOn": \[],

&nbsp;               "policy": {

&nbsp;                   "timeout": "0.12:00:00",

&nbsp;                   "retry": 0,

&nbsp;                   "retryIntervalInSeconds": 30,

&nbsp;                   "secureOutput": false,

&nbsp;                   "secureInput": false

&nbsp;               },

&nbsp;               "userProperties": \[],

&nbsp;               "typeProperties": {

&nbsp;                   "method": "GET",

&nbsp;                   "url": "\\thttps://dummy.restapiexample.com/api/v1/employees"

&nbsp;               }

&nbsp;           }

&nbsp;       ],

&nbsp;       "annotations": \[]

&nbsp;   }

}







**Pl\_wbactivity pipeline Output:**





{

&nbsp;	"status": "success",

&nbsp;	"data": \[

&nbsp;		{

&nbsp;			"id": 1,

&nbsp;			"employee\_name": "Tiger Nixon",

&nbsp;			"employee\_salary": 320800,

&nbsp;			"employee\_age": 61,

&nbsp;			"profile\_image": ""

&nbsp;		},

&nbsp;		{

&nbsp;			"id": 2,

&nbsp;			"employee\_name": "Garrett Winters",

&nbsp;			"employee\_salary": 170750,

&nbsp;			"employee\_age": 63,

&nbsp;			"profile\_image": ""

&nbsp;		},

&nbsp;		{

&nbsp;			"id": 3,

&nbsp;			"employee\_name": "Ashton Cox",

&nbsp;			"employee\_salary": 86000,

&nbsp;			"employee\_age": 66,

&nbsp;			"profile\_image": ""

&nbsp;		},

&nbsp;		{

&nbsp;			"id": 4,

&nbsp;			"employee\_name": "Cedric Kelly",

&nbsp;			"employee\_salary": 433060,

&nbsp;			"employee\_age": 22,

&nbsp;			"profile\_image": ""

&nbsp;		},

&nbsp;		{

&nbsp;			"id": 5,

&nbsp;			"employee\_name": "Airi Satou",

&nbsp;			"employee\_salary": 162700,

&nbsp;			"employee\_age": 33,

&nbsp;			"profile\_image": ""

&nbsp;		},

&nbsp;		{

&nbsp;			"id": 6,

&nbsp;			"employee\_name": "Brielle Williamson",

&nbsp;			"employee\_salary": 372000,

&nbsp;			"employee\_age": 61,

&nbsp;			"profile\_image": ""

&nbsp;		},

&nbsp;		{

&nbsp;			"id": 7,

&nbsp;			"employee\_name": "Herrod Chandler",

&nbsp;			"employee\_salary": 137500,

&nbsp;			"employee\_age": 59,

&nbsp;			"profile\_image": ""

&nbsp;		},

&nbsp;		{

&nbsp;			"id": 8,

&nbsp;			"employee\_name": "Rhona Davidson",

&nbsp;			"employee\_salary": 327900,

&nbsp;			"employee\_age": 55,

&nbsp;			"profile\_image": ""

&nbsp;		},

&nbsp;		{

&nbsp;			"id": 9,

&nbsp;			"employee\_name": "Colleen Hurst",

&nbsp;			"employee\_salary": 205500,

&nbsp;			"employee\_age": 39,

&nbsp;			"profile\_image": ""

&nbsp;		},

&nbsp;		{

&nbsp;			"id": 10,

&nbsp;			"employee\_name": "Sonya Frost",

&nbsp;			"employee\_salary": 103600,

&nbsp;			"employee\_age": 23,

&nbsp;			"profile\_image": ""

&nbsp;		},

&nbsp;		{

&nbsp;			"id": 11,

&nbsp;			"employee\_name": "Jena Gaines",

&nbsp;			"employee\_salary": 90560,

&nbsp;			"employee\_age": 30,

&nbsp;			"profile\_image": ""

&nbsp;		},

&nbsp;		{

&nbsp;			"id": 12,

&nbsp;			"employee\_name": "Quinn Flynn",

&nbsp;			"employee\_salary": 342000,

&nbsp;			"employee\_age": 22,

&nbsp;			"profile\_image": ""

&nbsp;		},

&nbsp;		{

&nbsp;			"id": 13,

&nbsp;			"employee\_name": "Charde Marshall",

&nbsp;			"employee\_salary": 470600,

&nbsp;			"employee\_age": 36,

&nbsp;			"profile\_image": ""

&nbsp;		},

&nbsp;		{

&nbsp;			"id": 14,

&nbsp;			"employee\_name": "Haley Kennedy",

&nbsp;			"employee\_salary": 313500,

&nbsp;			"employee\_age": 43,

&nbsp;			"profile\_image": ""

&nbsp;		},

&nbsp;		{

&nbsp;			"id": 15,

&nbsp;			"employee\_name": "Tatyana Fitzpatrick",

&nbsp;			"employee\_salary": 385750,

&nbsp;			"employee\_age": 19,

&nbsp;			"profile\_image": ""

&nbsp;		},

&nbsp;		{

&nbsp;			"id": 16,

&nbsp;			"employee\_name": "Michael Silva",

&nbsp;			"employee\_salary": 198500,

&nbsp;			"employee\_age": 66,

&nbsp;			"profile\_image": ""

&nbsp;		},

&nbsp;		{

&nbsp;			"id": 17,

&nbsp;			"employee\_name": "Paul Byrd",

&nbsp;			"employee\_salary": 725000,

&nbsp;			"employee\_age": 64,

&nbsp;			"profile\_image": ""

&nbsp;		},

&nbsp;		{

&nbsp;			"id": 18,

&nbsp;			"employee\_name": "Gloria Little",

&nbsp;			"employee\_salary": 237500,

&nbsp;			"employee\_age": 59,

&nbsp;			"profile\_image": ""

&nbsp;		},

&nbsp;		{

&nbsp;			"id": 19,

&nbsp;			"employee\_name": "Bradley Greer",

&nbsp;			"employee\_salary": 132000,

&nbsp;			"employee\_age": 41,

&nbsp;			"profile\_image": ""

&nbsp;		},

&nbsp;		{

&nbsp;			"id": 20,

&nbsp;			"employee\_name": "Dai Rios",

&nbsp;			"employee\_salary": 217500,

&nbsp;			"employee\_age": 35,

&nbsp;			"profile\_image": ""

&nbsp;		},

&nbsp;		{

&nbsp;			"id": 21,

&nbsp;			"employee\_name": "Jenette Caldwell",

&nbsp;			"employee\_salary": 345000,

&nbsp;			"employee\_age": 30,

&nbsp;			"profile\_image": ""

&nbsp;		},

&nbsp;		{

&nbsp;			"id": 22,

&nbsp;			"employee\_name": "Yuri Berry",

&nbsp;			"employee\_salary": 675000,

&nbsp;			"employee\_age": 40,

&nbsp;			"profile\_image": ""

&nbsp;		},

&nbsp;		{

&nbsp;			"id": 23,

&nbsp;			"employee\_name": "Caesar Vance",

&nbsp;			"employee\_salary": 106450,

&nbsp;			"employee\_age": 21,

&nbsp;			"profile\_image": ""

&nbsp;		},

&nbsp;		{

&nbsp;			"id": 24,

&nbsp;			"employee\_name": "Doris Wilder",

&nbsp;			"employee\_salary": 85600,

&nbsp;			"employee\_age": 23,

&nbsp;			"profile\_image": ""

&nbsp;		}

&nbsp;	],

&nbsp;	"message": "Successfully! All records has been fetched.",

&nbsp;	"ADFHttpStatusCodeInResponse": "200",

&nbsp;	"ADFWebActivityResponseHeaders": {

&nbsp;		"X-RateLimit-Limit": "60",

&nbsp;		"X-RateLimit-Remaining": "58",

&nbsp;		"Vary": "Accept-Encoding",

&nbsp;		"X-Server-Cache": "true",

&nbsp;		"X-Proxy-Cache": "MISS",

&nbsp;		"Transfer-Encoding": "chunked",

&nbsp;		"Cache-Control": "no-cache, private",

&nbsp;		"Date": "Wed, 15 Oct 2025 02:06:33 GMT",

&nbsp;		"Server": "nginx/1.25.5",

&nbsp;		"Content-Type": "application/json"

&nbsp;	},

&nbsp;	"effectiveIntegrationRuntime": "AutoResolveIntegrationRuntime (South India)",

&nbsp;	"executionDuration": 1,

&nbsp;	"durationInQueue": {

&nbsp;		"integrationRuntimeQueue": 1

&nbsp;	},

&nbsp;	"billingReference": {

&nbsp;		"activityType": "ExternalActivity",

&nbsp;		"billableDuration": \[

&nbsp;			{

&nbsp;				"meterType": "AzureIR",

&nbsp;				"duration": 0.016666666666666666,

&nbsp;				"unit": "Hours"

&nbsp;			}

&nbsp;		]

&nbsp;	}

}

