# Overview

 This project is a small direnv based _(.envrc)_ shell script to download basic everyday tools we use with kuberetes and setup a basic workspace while allows to isolate parameters and bins per worspace folder. The tools are enlisted below and are to be downloaded in a `bin/` folder.

# Prerequisites
 - Any Linux (amd64) distro.
 - [Direnv](https://direnv.net/)

# Tools   

The tools that are downloaded during env initialisation are:

 - [Kubectl](https://kubernetes.io/docs/reference/kubectl/kubectl/)
 - [CFSSL && CFSSL Json](https://github.com/cloudflare/cfssl)
 - [Kubectx \& Kubens](https://github.com/ahmetb/kubectx)
 - [Kubebox](https://github.com/astefanutti/kubebox/)
 - [Kubetail](https://github.com/johanhaleby/kubetail)
 - [Kubespy](https://github.com/pulumi/kubespy)

# Install

 To install the project you just need to copy the `.envrc` file in your workspace folder.

# Usage / Initialise workspace

 To initialise your workspace you need to run `direnv allow .` in the root folder. All tools are to be downloaded in the `bin/` folder and `PATH` env variable to to be updated.

 **NOTE:**
  Please not that `KUBECONFIG` env variable by defalt points to `${HOME}/.kube/config`

# License

```
  Copyright 2019 Ioannis Polyzos

  Licensed under the Apache License, Version 2.0 (the "License");
  you may not use this file except in compliance with the License.
  You may obtain a copy of the License at

      http://www.apache.org/licenses/LICENSE-2.0

  Unless required by applicable law or agreed to in writing, software
  distributed under the License is distributed on an "AS IS" BASIS,
  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
  See the License for the specific language governing permissions and
  limitations under the License.
```