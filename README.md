# Vertically Sliced .NET Serverless Lambdas

Presentation and instructions for setting up and running serverless AWS Lambda with .NET.

The presentation has links for the tools you need to setup. You can create the sample project using this:

```powershell
# Install the Lambda tools globally
dotnet tool install -g Amazon.Lambda.Tools

# Install the Lambda templates for dotnet new
dotnet new -i "Amazon.Lambda.Templates::*"

# Create a new project template
dotnet new serverless.DynamoDBBlogAPI -n ServerlessExample
```

This example is called "serverless" but is a different example from the [Serverless Framework](https://serverless.com/). This example uses CloudFormation from AWS instead to automate deployment. You may find the syntax and patterns of the Serverless Framework easier to follow, and you can drop down to CloudFormation if you need to do something that's not supported.

AWS also has documentation on [.NET Core CLI](https://docs.aws.amazon.com/lambda/latest/dg/lambda-dotnet-coreclr-deployment-package.html) that are helpful to get started and get your bearings around the templates.
