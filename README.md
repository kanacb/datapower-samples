# Datapower Templates
CodeBridge can be used to generate the code for IBM DataPower Gateway API js scripts by providing a set of templates and configurations that can be used to generate the desired code. The templates can be customized to the specific needs of the user, and the configurations can be used to control the generation of the code.

Here is a general overview of how CodeBridge can be used to generate the code for IBM DataPower Gateway API js scripts:

1. **Define the templates:** The first step is to define the templates that will be used to generate the code. The templates can be written in any programming language, but they should be structured in a way that is easy for CodeBridge to understand. The templates can include variables that will be replaced with values during the code generation process.

2. **Configure CodeBridge:** The next step is to configure CodeBridge to tell it how to generate the code. The configuration can include information such as the location of the templates, the location of the output files, and the values of the variables that will be replaced during the code generation process.

3. **Generate the code:** Once the templates and configuration are in place, CodeBridge can be used to generate the code. CodeBridge will process the templates and replace the variables with the appropriate values, and then generate the output files.

Here is an example of how CodeBridge can be used to generate the code for an IBM DataPower Gateway API js script that creates a new Gateway service:

```
// Define the template for the js script
template createServiceTemplate {
    var serviceName = "MyService";
    var serviceDescription = "This is my service";

    jsCode {
        var service = new DataPower.Service();
        service.name = serviceName;
        service.description = serviceDescription;

        serviceManager.createService(service);
    }
}

// Configure CodeBridge
CodeBridge.configure({
    templateDirectory: "templates",
    outputDirectory: "output",
    serviceName: "MyService",
    serviceDescription: "This is my service"
});

// Generate the code
CodeBridge.generateCode();
```

This code will generate a js script called `createService.js` that creates a new Gateway service named `MyService` with the description `This is my service`.

CodeBridge is a powerful tool that can be used to generate the code for a variety of tasks. By providing a set of templates and configurations, CodeBridge can be used to automate the code generation process, saving time and effort.

## B2B Routing

## JSON - reading from input
### Extra Context
### InputVars Context

## Error Handler

## Header Handler

## External
### Gateway
### XSL

## File Open Url

## Health Checker

## XML
### DOM
### xPath
### xslt
