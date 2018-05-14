# Dev
Document for FloGo Trigger developed by Team_Flogo

	Schema 
"outputs": [
{
"name": "Time-Occured",
"type": "string"
},
{
"name": "fullname",
"type": "string"
},
{
"name": "Filename",
"type": "string"
},
{
"name": "filepath",
"type": "string"
},
{
"name": "content",
"type": "string"
},
{
"name": "Size",
"type": "string"
},
{
"name": "LastModified",
"type": "string"
},
{
"name": "Action",
"type": "string"
}
],
"handler": {
"settings": [
{
"name": "FileName",
"type": "string",
"required" : true
},
{
"name": "Polling-Interval-Sec",
"type": "int",
"value": "5"
},
{
"name": "Include-Existing",
"type": "string",
"required" : true,
"allowed" : ["false", "true"]
},
{
"name": "Exclude-File-Content",
"type": "string",
"required" : true,
"allowed" : ["false", "true"]
}
]
}
}

	Working Flow:

 





	A sample Configuration: 
const testConfig string = `{
"id": "mytrigger",
"settings": {
    
},
"handlers": [
{
"actionId": "test_action",
"settings": {
                "FileName": "C:/Go_Workspace/test/activity.go",
                "Polling-Interval-Sec": "5",
                "Include-Existing": "false",
                "Exclude-File-Content": "false"
}
}
]
}`

