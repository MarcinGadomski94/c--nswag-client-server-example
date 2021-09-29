# C# NSwag Client/Server Generator Example

This example shows how to generate server and client code basing on *.yml files that contains
definition of the API.

Currently, project contains an examples for:
* Generation of Client code for OAS3;
* Generation of Server code for OAS3;

For code generation, NSwag package is being used. Client and Server code is being regenerated
basing on what is in *.yml file every time the project is built.

Code generation works on all operating systems.

This example also contains auto-generation of documentation file for Git repository in Markdown
using VSXMD package for Server side project.

Example is using .NET 5 framework.