**ci-reusable workflow.yml - Documentation**

This repo contains a ci-reusable workflow.yml pipeline where it has the following:

Workflow_call - Used as a reusable workflow.

Checkout:          Clones the code from github repo to the runner.

Unit test:         Checks the logic of the code.

Integration test:  Checks different connections(API,Service, database) are connected together or not.

Code coverage:     Check the coverage reports.

SBOM (Software Bill of Material): It lists out the lib, dependecny version, licience info.

Trivy:  Performs security vulnerbilitiy scanning.

Docker-Build:   Login to the github container registry.

Build and push:  Image is getting built and pushed to the container registry.

Cosign: It sigin to the container registry passwordless with OIDC and stores the signature in the registry.
