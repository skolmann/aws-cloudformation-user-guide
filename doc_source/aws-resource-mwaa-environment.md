# AWS::MWAA::Environment<a name="aws-resource-mwaa-environment"></a>

The `AWS::MWAA::Environment` resource\.

## Syntax<a name="aws-resource-mwaa-environment-syntax"></a>

To declare this entity in your AWS CloudFormation template, use the following syntax:

### JSON<a name="aws-resource-mwaa-environment-syntax.json"></a>

```
{
  "Type" : "AWS::MWAA::Environment",
  "Properties" : {
      "[AirflowConfigurationOptions](#cfn-mwaa-environment-airflowconfigurationoptions)" : AirflowConfigurationOptions,
      "[AirflowVersion](#cfn-mwaa-environment-airflowversion)" : String,
      "[DagS3Path](#cfn-mwaa-environment-dags3path)" : String,
      "[EnvironmentClass](#cfn-mwaa-environment-environmentclass)" : String,
      "[ExecutionRoleArn](#cfn-mwaa-environment-executionrolearn)" : String,
      "[KmsKey](#cfn-mwaa-environment-kmskey)" : String,
      "[LoggingConfiguration](#cfn-mwaa-environment-loggingconfiguration)" : LoggingConfiguration,
      "[MaxWorkers](#cfn-mwaa-environment-maxworkers)" : Integer,
      "[NetworkConfiguration](#cfn-mwaa-environment-networkconfiguration)" : NetworkConfiguration,
      "[PluginsS3ObjectVersion](#cfn-mwaa-environment-pluginss3objectversion)" : String,
      "[PluginsS3Path](#cfn-mwaa-environment-pluginss3path)" : String,
      "[RequirementsS3ObjectVersion](#cfn-mwaa-environment-requirementss3objectversion)" : String,
      "[RequirementsS3Path](#cfn-mwaa-environment-requirementss3path)" : String,
      "[SourceBucketArn](#cfn-mwaa-environment-sourcebucketarn)" : String,
      "[Tags](#cfn-mwaa-environment-tags)" : TagMap,
      "[WebserverAccessMode](#cfn-mwaa-environment-webserveraccessmode)" : String,
      "[WebserverUrl](#cfn-mwaa-environment-webserverurl)" : String,
      "[WeeklyMaintenanceWindowStart](#cfn-mwaa-environment-weeklymaintenancewindowstart)" : String
    }
}
```

### YAML<a name="aws-resource-mwaa-environment-syntax.yaml"></a>

```
Type: AWS::MWAA::Environment
Properties: 
  [AirflowConfigurationOptions](#cfn-mwaa-environment-airflowconfigurationoptions): 
    AirflowConfigurationOptions
  [AirflowVersion](#cfn-mwaa-environment-airflowversion): String
  [DagS3Path](#cfn-mwaa-environment-dags3path): String
  [EnvironmentClass](#cfn-mwaa-environment-environmentclass): String
  [ExecutionRoleArn](#cfn-mwaa-environment-executionrolearn): String
  [KmsKey](#cfn-mwaa-environment-kmskey): String
  [LoggingConfiguration](#cfn-mwaa-environment-loggingconfiguration): 
    LoggingConfiguration
  [MaxWorkers](#cfn-mwaa-environment-maxworkers): Integer
  [NetworkConfiguration](#cfn-mwaa-environment-networkconfiguration): 
    NetworkConfiguration
  [PluginsS3ObjectVersion](#cfn-mwaa-environment-pluginss3objectversion): String
  [PluginsS3Path](#cfn-mwaa-environment-pluginss3path): String
  [RequirementsS3ObjectVersion](#cfn-mwaa-environment-requirementss3objectversion): String
  [RequirementsS3Path](#cfn-mwaa-environment-requirementss3path): String
  [SourceBucketArn](#cfn-mwaa-environment-sourcebucketarn): String
  [Tags](#cfn-mwaa-environment-tags): 
    TagMap
  [WebserverAccessMode](#cfn-mwaa-environment-webserveraccessmode): String
  [WebserverUrl](#cfn-mwaa-environment-webserverurl): String
  [WeeklyMaintenanceWindowStart](#cfn-mwaa-environment-weeklymaintenancewindowstart): String
```

## Properties<a name="aws-resource-mwaa-environment-properties"></a>

`AirflowConfigurationOptions`  <a name="cfn-mwaa-environment-airflowconfigurationoptions"></a>
The custom configuration options to use to override default Apache Airflow configuration options in your environment\.  
*Required*: No  
*Type*: [AirflowConfigurationOptions](aws-properties-mwaa-environment-airflowconfigurationoptions.md)  
*Update requires*: [No interruption](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/using-cfn-updating-stacks-update-behaviors.html#update-no-interrupt)

`AirflowVersion`  <a name="cfn-mwaa-environment-airflowversion"></a>
The version of Apache Airflow to use for the environment\.  
*Required*: No  
*Type*: String  
*Update requires*: [No interruption](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/using-cfn-updating-stacks-update-behaviors.html#update-no-interrupt)

`DagS3Path`  <a name="cfn-mwaa-environment-dags3path"></a>
The path to the DAGs folder in the S3 bucket\.  
*Required*: No  
*Type*: String  
*Update requires*: [No interruption](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/using-cfn-updating-stacks-update-behaviors.html#update-no-interrupt)

`EnvironmentClass`  <a name="cfn-mwaa-environment-environmentclass"></a>
The instance class to use to create the environment\.  
*Required*: No  
*Type*: String  
*Update requires*: [No interruption](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/using-cfn-updating-stacks-update-behaviors.html#update-no-interrupt)

`ExecutionRoleArn`  <a name="cfn-mwaa-environment-executionrolearn"></a>
The ARN of the IAM role to use as the execution role for the environment\.  
*Required*: No  
*Type*: String  
*Update requires*: [No interruption](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/using-cfn-updating-stacks-update-behaviors.html#update-no-interrupt)

`KmsKey`  <a name="cfn-mwaa-environment-kmskey"></a>
  
*Required*: No  
*Type*: String  
*Update requires*: [No interruption](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/using-cfn-updating-stacks-update-behaviors.html#update-no-interrupt)

`LoggingConfiguration`  <a name="cfn-mwaa-environment-loggingconfiguration"></a>
Specifies the logging settings for the environment\.  
*Required*: No  
*Type*: [LoggingConfiguration](aws-properties-mwaa-environment-loggingconfiguration.md)  
*Update requires*: [No interruption](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/using-cfn-updating-stacks-update-behaviors.html#update-no-interrupt)

`MaxWorkers`  <a name="cfn-mwaa-environment-maxworkers"></a>
The maximum number of workers to scale up to in the environment\.  
*Required*: No  
*Type*: Integer  
*Update requires*: [No interruption](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/using-cfn-updating-stacks-update-behaviors.html#update-no-interrupt)

`NetworkConfiguration`  <a name="cfn-mwaa-environment-networkconfiguration"></a>
  
*Required*: No  
*Type*: [NetworkConfiguration](aws-properties-mwaa-environment-networkconfiguration.md)  
*Update requires*: [Replacement](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/using-cfn-updating-stacks-update-behaviors.html#update-replacement)

`PluginsS3ObjectVersion`  <a name="cfn-mwaa-environment-pluginss3objectversion"></a>
The version of the plugins\.zip in file to use from the S3 bucket\.  
*Required*: No  
*Type*: String  
*Update requires*: [No interruption](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/using-cfn-updating-stacks-update-behaviors.html#update-no-interrupt)

`PluginsS3Path`  <a name="cfn-mwaa-environment-pluginss3path"></a>
The S3 URI to the plugins\.zip file to use for the environment\.  
*Required*: No  
*Type*: String  
*Update requires*: [No interruption](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/using-cfn-updating-stacks-update-behaviors.html#update-no-interrupt)

`RequirementsS3ObjectVersion`  <a name="cfn-mwaa-environment-requirementss3objectversion"></a>
The version of the requirements\.txt in file to use from the S3 bucket\.  
*Required*: No  
*Type*: String  
*Update requires*: [No interruption](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/using-cfn-updating-stacks-update-behaviors.html#update-no-interrupt)

`RequirementsS3Path`  <a name="cfn-mwaa-environment-requirementss3path"></a>
The S3 URI to the requirements\.txt file to use for the environment\.  
*Required*: No  
*Type*: String  
*Update requires*: [No interruption](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/using-cfn-updating-stacks-update-behaviors.html#update-no-interrupt)

`SourceBucketArn`  <a name="cfn-mwaa-environment-sourcebucketarn"></a>
The ARN of the S3 bucket to use to store your DAGs and associated support files for the environment\.  
*Required*: No  
*Type*: String  
*Update requires*: [No interruption](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/using-cfn-updating-stacks-update-behaviors.html#update-no-interrupt)

`Tags`  <a name="cfn-mwaa-environment-tags"></a>
  
*Required*: No  
*Type*: [TagMap](aws-properties-mwaa-environment-tagmap.md)  
*Update requires*: [No interruption](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/using-cfn-updating-stacks-update-behaviors.html#update-no-interrupt)

`WebserverAccessMode`  <a name="cfn-mwaa-environment-webserveraccessmode"></a>
  
*Required*: No  
*Type*: String  
*Update requires*: [No interruption](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/using-cfn-updating-stacks-update-behaviors.html#update-no-interrupt)

`WebserverUrl`  <a name="cfn-mwaa-environment-webserverurl"></a>
The URL to access the Apache Airflow UI in the environment\.  
*Required*: No  
*Type*: String  
*Update requires*: [No interruption](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/using-cfn-updating-stacks-update-behaviors.html#update-no-interrupt)

`WeeklyMaintenanceWindowStart`  <a name="cfn-mwaa-environment-weeklymaintenancewindowstart"></a>
The day and time of the week to start weekly maintenance updates of your environment, in the format DAY:HH:MM, such as TUE:03:30\. You can specify a start time in 30 minute increments only\. Supported input includes the following: MON\|TUE\|WED\|THU\|FRI\|SAT\|SUN:\(\[01\]\\\\d\|2\[0\-3\]\):\(00\|30\)  
*Required*: No  
*Type*: String  
*Update requires*: [No interruption](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/using-cfn-updating-stacks-update-behaviors.html#update-no-interrupt)

## Return values<a name="aws-resource-mwaa-environment-return-values"></a>

### Ref<a name="aws-resource-mwaa-environment-return-values-ref"></a>

### Fn::GetAtt<a name="aws-resource-mwaa-environment-return-values-fn--getatt"></a>

#### <a name="aws-resource-mwaa-environment-return-values-fn--getatt-fn--getatt"></a>

`Arn`  <a name="Arn-fn::getatt"></a>
Not currently supported by AWS CloudFormation\.

`CreatedAt`  <a name="CreatedAt-fn::getatt"></a>
Not currently supported by AWS CloudFormation\.

`LastUpdate`  <a name="LastUpdate-fn::getatt"></a>
Not currently supported by AWS CloudFormation\.

`Name`  <a name="Name-fn::getatt"></a>
Not currently supported by AWS CloudFormation\.

`ServiceRoleArn`  <a name="ServiceRoleArn-fn::getatt"></a>
Not currently supported by AWS CloudFormation\.

`Status`  <a name="Status-fn::getatt"></a>
Not currently supported by AWS CloudFormation\.