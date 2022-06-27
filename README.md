# Overview

This is a **template** sample application written in Java. It should be use as an app accelerator base template.

## Critical Files

The following is a list of critical files utilized in the conventions for building
an Anthos application.

| File/Folder   |      Description      |  Required  |
|:-------------:|:----------------------|-----------:|
| Dockerfile :whale: |  File used to create the Docker image (built with kaniko) | :white_check_mark: |
| skaffold.yaml |  Used in local development to keep development environment in sync with changes. If not using skaffold, this file is optional (but recommended) |  :white_large_square: |
| build/ | CI/CD Pipeline setup to build to inherit the conventions for the development organization/ecosystem | :white_check_mark: |
| deploy/ | Cloud Build Deployment pipeline files | 
| k8s/ | Folder containing the Kubernetes resource manifests for "test", "stage" and "prod". Resource files are configured to use Kustomize during the CICD build. | :white_check_mark: |

## Placeholders to change

| File/Folder | Placeholder name | Notes |
|:-------------:|:----------------------|-----------:|
| org | Organization name | n/a |
| appname-package | application package | n/a |
| appname-class | application main class name | n/a |
| APP-NAME | placeholder in Yaml files | n/a |

## Licensing

```lang-none
Copyright 2022 Google LLC

Licensed under the Apache License, Version 2.0 (the "License");
you may not use this file except in compliance with the License.
You may obtain a copy of the License at

    https://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing, software
distributed under the License is distributed on an "AS IS" BASIS,
WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
See the License for the specific language governing permissions and
limitations under the License.
```

## Usage

Copyright 2022 Google. This software is shared as sample code and not intended
for production use and provided as-is, without warranty or representation for
any use or purpose. Your use of it is discretionary and subject to your
agreement with Google.

## Contributing

*   [Contributing guidelines][contributing-guidelines]
