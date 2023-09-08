offy-pack-azure-function
========================

The offy-pack as a serverless Azure function.


Deployment with GitHub Actions
------------------------------

__offy-pack-azure-function__ supports GitHub Actions to build and deploy to Azure automatically following a push to the master branch.  This workflow can also be triggered manually from the Actions tab.

The Actions require the following variables/secrets:
- `AZURE_FUNCTIONAPP_NAME` (ex: offy-pack-example) as an Actions Variable
- `SCM_CREDENTIALS` as an Actions Secret

The `SCM_CREDENTIALS` can be retrieved from the Azure Portal as follows:
- browse to the Function App
- select _Get publish profile_ from the Overview page
- save the .PublishSettings file
- under the Settings tab of this GitHub repository, select Security - Secrets and Variables - Actions
- create a _New repository secret_ called `SCM_CREDENTIALS` and paste in the contents of the file


License
-------

MIT License

Copyright (c) 2023 Offy

Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR 
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, 
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE 
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER 
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, 
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN 
THE SOFTWARE.