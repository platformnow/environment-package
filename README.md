# PlatformNOW Environment Package

The environment package provides crossplane compositions to install a namespace and add gitops to it.


## Installation

```bash
kubectl apply -f packages/package.yaml
```
## Usage

Now you can apply the desired XR. For example, to install an environment:

```bash
kubectl apply -f defaults/environment.yaml
```
**NOTE
This will add gitops from the root of the repository. If you want to use a different path, you can change the path in the XR.

Examples of other XR's can be found in the [examples](examples) folder.

## Publishing

Github Actions is used to build and publish the package. The following steps can be performed:

1. Create a tag

```bash 
git tag v0.0.1 -m "Release v0.0.1"
```

2. Push the tag

```bash
git push --tags
```
