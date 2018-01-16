# Getting started

An API for securitytext.org

## How to Build

The generated code uses a few Gradle dependencies e.g., Jackson, Volley,
and Apache HttpClient. The reference to these dependencies is already
added in the build.gradle file will be installed automatically. Therefore,
you will need internet access for a successful build.

* In order to open the client library in Android Studio click on ``` Open an Existing Android Project ```.

![Importing SDK into Android Studio - Step 1](https://apidocs.io/illustration/android?step=import1&workspaceFolder=securitytext.org%20API&workspaceName=SecuritytextOrgAPI&projectName=SecuritytextOrgAPILib&rootNamespace=org.securitytext.api)

* Browse to locate the folder containing the source code. Select the location of the SecuritytextOrgAPI gradle project and click ``` Ok ```.

![Importing SDK into Android Studio - Step 2](https://apidocs.io/illustration/android?step=import2&workspaceFolder=securitytext.org%20API&workspaceName=SecuritytextOrgAPI&projectName=SecuritytextOrgAPILib&rootNamespace=org.securitytext.api)

* Upon successful import, the project can be built by clicking on ``` Build > Make Project ``` or  pressing ``` Ctrl + F9 ```.

![Importing SDK into Android Studio - Step 3](https://apidocs.io/illustration/android?step=import3&workspaceFolder=securitytext.org%20API&workspaceName=SecuritytextOrgAPI&projectName=SecuritytextOrgAPILib&rootNamespace=org.securitytext.api)

## How to Use

The following section explains how to use the SecuritytextOrgAPI library in a new project.

### 1. Starting a new project 

For starting a new project, click on ``` Create New Android Studio Project ```.

![Add a new project in Android Studio - Step 1](https://apidocs.io/illustration/android?step=createNewProject0&workspaceFolder=securitytext.org%20API&workspaceName=SecuritytextOrgAPI&projectName=SecuritytextOrgAPILib&rootNamespace=org.securitytext.api)

Here, configure the new project by adding the name, domain and location of the sample application followed by clicking ``` Next ```.

![Create a new Android Studio Project - Step 2](https://apidocs.io/illustration/android?step=createNewProject1&workspaceFolder=securitytext.org%20API&workspaceName=SecuritytextOrgAPI&projectName=SecuritytextOrgAPILib&rootNamespace=org.securitytext.api)

Following this, select the `Phone and Tablet` option as shown in the illustration below and click `Next`.

![Create a new Android Studio Project - Step 3](https://apidocs.io/illustration/android?step=createNewProject2&workspaceFolder=securitytext.org%20API&workspaceName=SecuritytextOrgAPI&projectName=SecuritytextOrgAPILib&rootNamespace=org.securitytext.api)

In the following step, choose ``` Empty Activity ``` as the activity type and click ``` Next ```.

![Create a new Android Studio Project - Step 4](https://apidocs.io/illustration/android?step=createNewProject3&workspaceFolder=securitytext.org%20API&workspaceName=SecuritytextOrgAPI&projectName=SecuritytextOrgAPILib&rootNamespace=org.securitytext.api)

In this step, provide an ``` Activity Name ``` and ``` Layout Name ``` and click ``` Finish ```.  This would take you to the newly created project.

![Create a new Android Studio Project - Step 4](https://apidocs.io/illustration/android?step=createNewProject4&workspaceFolder=securitytext.org%20API&workspaceName=SecuritytextOrgAPI&projectName=SecuritytextOrgAPILib&rootNamespace=org.securitytext.api)

### 2. Add reference of the library project

In order to add a dependency to this sample application, click on the android button shown in the project explorer on the left side as shown in the picture. Click on ``` Project ``` in the drop down that emerges.  

![Adding dependency to the client library - Step 1](https://apidocs.io/illustration/android?step=testProject0&workspaceFolder=securitytext.org%20API&workspaceName=SecuritytextOrgAPI&projectName=SecuritytextOrgAPILib&rootNamespace=org.securitytext.api)

Right click the sample application in the project explorer and click on ``` New > Module ```  as shown in the picture.

![Adding dependency to the client library - Step 2](https://apidocs.io/illustration/android?step=testProject1&workspaceFolder=securitytext.org%20API&workspaceName=SecuritytextOrgAPI&projectName=SecuritytextOrgAPILib&rootNamespace=org.securitytext.api)

Choose ``` Import Gradle Project ``` and click ``` Next ```.

![Adding dependency to the client library - Step 3](https://apidocs.io/illustration/android?step=testProject2&workspaceFolder=securitytext.org%20API&workspaceName=SecuritytextOrgAPI&projectName=SecuritytextOrgAPILib&rootNamespace=org.securitytext.api)

Click on ``` Finish ``` which would take you back to the sample application with the refernced SDK. 

![Adding dependency to the client library - Step 4](https://apidocs.io/illustration/android?step=testProject3&workspaceFolder=securitytext.org%20API&workspaceName=SecuritytextOrgAPI&projectName=SecuritytextOrgAPILib&rootNamespace=org.securitytext.api)

In the following step naigate to the ``` SampleApplication >  app > build.gradle ``` file and add the following line ```compile project(path: ':SecuritytextOrgAPI')``` to the dependencies section as shown in the illustration below.

![Adding dependency to the client library - Step 5](https://apidocs.io/illustration/android?step=testProject4&workspaceFolder=securitytext.org%20API&workspaceName=SecuritytextOrgAPI&projectName=SecuritytextOrgAPILib&rootNamespace=org.securitytext.api)

Finally, press ``` Sync Now ``` in the warning visible as shown in the picture below.

![Adding dependency to the client library - Step 6](https://apidocs.io/illustration/android?step=testProject5&workspaceFolder=securitytext.org%20API&workspaceName=SecuritytextOrgAPI&projectName=SecuritytextOrgAPILib&rootNamespace=org.securitytext.api)

### 3. Write sample code

Once the ``` SampleApplication ``` is created, a file named ``` SampleApplication > app > src > main > java > MainActivity ``` will be visible in the *Project Explorer* with an ``` onCreate ``` method. This is the entry point for the execution of the created project.
Here, you can add code to initialize the client library and instantiate a *Controller* class. Sample code to initialize the client library and using controller methods is given in the subsequent sections.

## How to Test

The generated code and the server can be tested using automatically generated test cases. 
JUnit is used as the testing framework and test runner.

In Android Studio, for running the tests do the following:

1. Right click on *SampleApplication > SecuritytextOrgAPILib > androidTest > java)* from the project explorer.
2. Select "Run All Tests" or use "Ctrl + Shift + F10" to run the Tests.

## Initialization

### 

API client can be initialized as following. The `appContext` being passed is the Android application [`Context`](https://developer.android.com/reference/android/content/Context.html).

```java

org.securitytext.api.Configuration.initialize(appContext);
SecuritytextOrgAPIClient client = new SecuritytextOrgAPIClient();
```


# Class Reference

## <a name="list_of_controllers"></a>List of Controllers

* [WhoisController](#whois_controller)

## <a name="whois_controller"></a>![Class: ](https://apidocs.io/img/class.png "org.securitytext.api.controllers.WhoisController") WhoisController

### Get singleton instance

The singleton instance of the ``` WhoisController ``` class can be accessed from the API Client.

```java
WhoisController whois = client.getWhois();
```

### <a name="create_api_whois_query_async"></a>![Method: ](https://apidocs.io/img/method.png "org.securitytext.api.controllers.WhoisController.createApiWhoisQueryAsync") createApiWhoisQueryAsync

> *Tags:*  ``` Skips Authentication ``` 

> Query the server for a Domain object


```java
void createApiWhoisQueryAsync(
        final RequestsQueryModel body,
        final APICallBack<ResponsesQueryModel> callBack)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | Body of API request |


#### Example Usage

```java
try {
    RequestsQueryModel body = new RequestsQueryModel();
    // Invoking the API call with sample inputs
    whois.createApiWhoisQueryAsync(body, new APICallBack<ResponsesQueryModel>() {
        public void onSuccess(HttpContext context, ResponsesQueryModel response) {
            // TODO success callback handler
        }
        public void onFailure(HttpContext context, Throwable error) {
            // TODO failure callback handler
        }
    });
} catch(JsonProcessingException e) {
    // TODO Auto-generated catch block
    e.printStackTrace();
}
```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 400 | Bad Request |
| 406 | Not Acceptable |
| 500 | Internal Server Error |



[Back to List of Controllers](#list_of_controllers)



