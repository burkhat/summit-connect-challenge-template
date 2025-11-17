# Red Hat Summit Connect Challenge on Developer Hub

A Backstage Golden Path Template to deploy an example application via ArgoCD.

Content:

- Simple [Golden Path Template](template.yaml)
- Component [Catalog Info](./skeleton/catalog-info.yaml)
- [Helm chart](./manifests/helm/summit-connect-challenge/) for the example application deployment:
- ArgoCD [Application](./manifests/argocd/application.yaml)

## Usage

First of all: fork this repository! You need to make changes to it to work!

Once done: add 2 parameters into the `template.yaml`, `name` and `title`. You want to add them to `metadata`, next to where `description` is present.
`name` should be a unique identifier and `title` is how it's going to be shown in Developer Hub

Then: to make use of this template and therefore be able to deploy the application via Developer Hub, you need to add this template first. To do so:

- Be on the Developer Hub WebUI
- Navigate to 'Create'
- Press on "Register Existing Component'
- Enter the URL of this repository directly to the [template.yaml](template.yaml)
- Press on 'Analyze' and navigate the process until the end

## Challenge

This challenge is about navigating in Developer Hub and understanding how the templating works. If done correctly, this template will deploy the manifests in a way that you can access the deployed application and the flag will be revealed!
