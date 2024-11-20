# Runpad - Codemagic Example iOS

This repository demonstrates the integration of [Bytesalt Runpad](https://bytesalt.com/) with Codemagic for an iOS app.

## Setup

1. Generate CI client credentials by following the [CI Integration guide](https://bytesalt.com/docs/runpad/ci-integration/generate-ci-client-credentials). Note the Project ID as per the guide.
2. Store the generated credentials as Secure environment variables on Codemagic under a new group called `runpad-credentials`
    - `RUNPAD_CLIENT_ID`
    - `RUNPAD_CLIENT_SECRET`
  
  Refer to [this Codemagic documentation](https://docs.codemagic.io/yaml-basic-configuration/configuring-environment-variables/) for detailed instructions.

3. Store the fololowing Runpad options as environment variables on Codemagic under a new group called `runpad-options`
    - `RUNPAD_PROJECT_ID` : Project ID as you noted in the first step.
    - `RUNPAD_DEVICE` : Device you want to run tests on. For example, `iPhone 16`

4. Check the codemagic.yaml file for a reference configuration.
