
Credits to OpHoperHPO for making the image background remove tool https://github.com/OPHoperHPO/image-background-remove-tool


# remove_background_function
In this repository you can find an Azure Function, which listens to http requests, with which you can remove the background of an image. You can find an explanation here https://www.youtube.com/watch?v=0p6Q15ks7Dw&feature=youtu.be

In a consumption tier function, the startup time is around 30 seconds. An image of 1000x1000px takes about 3 seconds to process.

##This is not production ready. 

TODO: 
-Code cleanup

-Reduce RAM usage <- larger files can timeout azure function

-Improve performance on lower images

-Allow API consumer to select pre/postprocessing methods

HOW TO DEPLOY THIS:
Create function app in Azure using Azure Portal OR Function CLI tools OR VS Code Azure Function plugin
Then deploy using CLI or VSCode
`func azure functionapp publish <FunctionAppName>` 
https://docs.microsoft.com/en-us/azure/azure-functions/functions-run-local?tabs=v4%2Cwindows%2Ccsharp%2Cportal%2Cbash%2Ckeda
