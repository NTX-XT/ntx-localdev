# Introduction

A local development server to host your Nintex form plugins. The server has CORS configured and provides a dummy certificate to enable SSL. For better security, please replace the provided certificate with your own.

# Installation

Install the server globally using `npm i @nintex/form-plugin-localdev -g` or locally using `npm i @nintex/form-plugin-localdev`

# How to use

The server takes two parameters:
- `-folder (or -f)`: Specifies the path of the files files to be servers. This parameter is required.
- `-port (or -p)`: Specify the port. If not specified, the port 8888 will be used by default.

When globally installed, the server can be run using `ntx-localdev`. For local installs, run `npx ntx-localdev`

# Examples

- Serve the files under the project's dist folder on the default port: `ntx-localdev -f ./dist`
- Serve the files under the project's dist folder on port 8880: `ntx-localdev -f ./dist -p 8880`

The server is used by the Ninhtex Form Plugin Starter Kit, both the typescript and the javascript flavours. Please refer to those repos for more working scenarios.

