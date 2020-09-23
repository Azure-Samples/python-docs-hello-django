---
page_type: sample
description: "A minimal sample app that can be used to demonstrate deploying Django apps to Azure App Service on Linux."
languages:
- python
products:
- azure
- azure-app-service
---

# Python Django sample for Azure App Service (Linux)

This is a minimal Django app, without a database, that can be deployed to Azure App Service on Linux.

For instructions on running and deploying the code, see [Quickstart: Create a Python app in Azure App Service on Linux](https://docs.microsoft.com/azure/app-service/quickstart-python).

## Changes to Django settings

This sample contains two modifications in the file *django_hello/settings.py*:

- `ALLOWED_HOSTS` is set to include the value of the `WEBSITE_HOSTNAME` environment variable, if present. Azure App Service automatically sets this environment variable upon deployment to the app's URL.

- The `DATABASES` object is commented out (using """) so that the app doesn't attempt to use a database at all. To use a database, remove the comments and modify the values as appropriate for your database.

## Contributing

This project has adopted the [Microsoft Open Source Code of Conduct](https://opensource.microsoft.com/codeofconduct/). For more information see the [Code of Conduct FAQ](https://opensource.microsoft.com/codeofconduct/faq/) or contact [opencode@microsoft.com](mailto:opencode@microsoft.com) with any additional questions or comments.
