# awesome-kubectl-plugins [![Awesome](https://cdn.rawgit.com/sindresorhus/awesome/d7305f38d29fed78fa85652e3a63e154dd8e8829/media/badge.svg)](https://github.com/sindresorhus/awesome) <img alt="PRs Welcome" src="https://img.shields.io/badge/PRs-welcome-brightgreen.svg" />

A curated list of awesome `kubectl` plugins inspired by the [awesome](https://github.com/sindresorhus/awesome) list.

If you see a link that isn't a good fit, you can fix it by submitting a pull request to help improve the list. Likewise, if you'd like to add or fix something, click the [README.md](README.md) file to edit and submit a pull request.  Thank you!

## What are kubectl plugins?

> Since version 1.12, kubectl includes a plugin mechanism that allows you to extend kubectl with custom commands. Extending `kubectl` with plugins greatly enhances the productivity while using the CLI.

# Contents

* [Package Manager](#package-manager)
* [Resources](#resources)
* [Blog Posts](#blog-posts)
* [kubectl Plugins](#kubectl-plugins)

## Package Manager 📦
 * [Krew](https://github.com/kubernetes-sigs/krew)

## Resources
* [Writing Kubectl Plugins for Everyone](https://www.youtube.com/watch?v=83ITOTsXsHU)
* [Podcast - kubectl Plugins and krew, with Ahmet Alp Balkan and Luk Burchard](https://kubernetespodcast.com/episode/066-kubectl-plugins-and-krew/)

## Blog Posts

* [How to write a kubectl plugin](https://elsesiy.com/blog/how-to-kubectl-plugin)
* [Extending kubectl with plugins](https://kubernetes.io/docs/tasks/extend-kubectl/kubectl-plugins/)
* [Write your own kubectl subcommands](https://ahmet.im/blog/kubectl-plugins/)
* [Manage Kubernetes Plugins with Krew](https://thepracticalsysadmin.com/manage-kubernetes-plugins-with-krew/)
* [Boosting Your Kubectl Productivity](https://learnk8s.io/blog/kubectl-productivity/)
* [Top 15 Kubectl plugins for security engineers](https://sysdig.com/blog/top-15-kubectl-plugins-for-security-engineers/)

## Use `awesome-kubectl-plugins` as a Custom Index via Krew

A notable feature `custom index` was added in `krew's` [v0.4.0](https://github.com/kubernetes-sigs/krew/releases/tag/v0.4.0) release. This means you can now use custom indexes of your own to install the plugins via `krew`.

Was you plugin not accepted in default `krew-index` due to some reasons? No issues, you can still use that plugin manifest in your custom index and install it via krew. 

Now, `awesome-kubectl-plugins` is not just a list of awesome kubectl plugins (without any centralised control), you can actually use this to add your own plugins like you did for `krew-index` and install them locally. :rocket:

**Note**: This does not mean you can install plugins without a valid `plugins.yaml` for your plugin. You still need to have a plugin manifest. 

### How to add your plugin to awesome-kubectl-plugins
* Add your plugin's name, description and category to the below [kubectl Plugins](#kubectl-plugins) list.
* Add `plugin-name.yaml` manifest to `./plugins` directory.
* And, you're done.
 
### Installing plugins via awesome-kubectl-plugins
* Add the custom index to krew:
  ```
  $ kubectl krew index add awesome-kubectl-plugins https://github.com/ishantanu/awesome-kubectl-plugins.git
  ```
* Install a plugin from the custom index by running:
  ```
  kubectl krew install awesome-kubectl-plugins/access-matrix
  ```
  
## kubectl Plugins

| No. | Plugin                                                            | Description                                                                             | Category |
| --- | ----------------------------------------------------------------- | -------------------------------------------- | -------- |
| 1   | [rakkess](https://github.com/corneliusweig/rakkess)                                | Review Access - kubectl plugin to show an access matrix for k8s server resources                | RBAC                |
| 2   | [kubectl-who-can](https://github.com/aquasecurity/kubectl-who-can)                 | Show who has RBAC permissions to perform actions on different resources in Kubernetes        | RBAC                |
| 3   | [kubectl-lint](https://github.com/SethCurry/kubectl-lint)                          | A kubectl plugin to perform linting                                                              | Linting             |
| 4   | [kubectl-neat](https://github.com/itaysk/kubectl-neat)                             | Clean up Kuberntes yaml and json output to make it readable                              | Linting             |
| 5   | [ksort](https://github.com/superbrothers/ksort)                                    | Sort manifest files in a proper order by Kind                                                 | Linting             |
| 6   | [kubectl-debug](https://github.com/aylei/kubectl-debug)                            | Debug your pod by a new container with every troubleshooting tools pre-installed               | Debugging           |
| 7   | [kube-profefe](https://github.com/profefe/kube-profefe)                            | continuous profiling made easy in Kubernetes with profefe                                  | Debugging           |
| 8   | [ksniff](https://github.com/eldadru/ksniff)                                        | Kubectl plugin to ease sniffing on kubernetes pods using tcpdump and wireshark                 | Networking          |
| 9   | [kubectl-swiftnp](https://github.com/bmuschko/kubectl-swiftnp)                     | A kubectl plugin for rendering details of Network Policies.                                      | Networking          |
| 10  | [kubectl-trace](https://github.com/iovisor/kubectl-trace)                          | Schedule bpftrace programs on your kubernetes cluster using the kubectl                  | Networking          |
| 11  | [kubectl-capture](https://github.com/sysdiglabs/kubectl-capture)                   | A kubectl plugin which triggers a Sysdig capture https://sysdig.com/opensource/inspect/          | Networking          |
| 12  | [kubectl-plugin-pvc](https://github.com/fabiand/kubectl-plugin-pvc)                | A simple kubectl binary plugin for PVC operations                                                | Storage             |
| 13  | [kubectl-dfi](https://github.com/makocchi-git/kubectl-dfi)                         | List and show disk resources of images on Kubernetes nodes.                                   | Storage             |
| 14  | [kubectl-unbound-pvc](https://github.com/ishantanu/kubectl-unbound-pvc)            | List and show disk resources of images on Kubernetes nodes.                                   | Storage             |
| 15  | [kubectl-df-pv](https://github.com/yashbhutwala/kubectl-df-pv)                     | giving admins df (disk free) like utility for persistent volumes                                 | Storage             |
| 16  | [outdated](https://github.com/replicatedhq/outdated)                               | Find and report outdated images running in a Kubernetes cluster                                 | Security            |
| 17  | [kubectl-kubesec](https://github.com/controlplaneio/kubectl-kubesec)               | Security risk analysis for Kubernetes resources https://kubesec.io                            | Security            |
| 18  | [duplik8s](https://github.com/Telemaco019/duplik8s)                                | Duplicate Pods with overriden commands and configurations. | Exec
| 19  | [kubectl-enter](https://github.com/kvaps/kubectl-enter)                            | Exec into node via kubectl                                                                     | Exec                |
| 20  | [kubectl-iexec](https://github.com/gabeduke/kubectl-iexec)                         | Kubectl plugin to interactively exec into a pod                                                | Exec                |
| 21  | [kubectl-ssh](https://github.com/IuryAlves/kubectl-ssh)                            | A kubectl plugin to ssh into a pod's node                                                        | Exec                |
| 22  | [kubectl-kcn](https://github.com/marjamis/kubectl-kcn)                             | A script and kubectl plugin which makes it easier to ssh into nodes within your cluster.     | Exec                |
| 23  | [duyguserbest kubectl-iexec](https://github.com/duyguserbest/kubectl-iexec)        | A script and kubectl plugin which makes it easier to ssh into nodes within your cluster.     | Exec                |
| 24  | [kubectl-exec-all](https://github.com/jpdasma/kubectl-exec-all)                    | kubectl plugin to execute a command in all running pods of a resource.                         | Exec                |
| 25  | [kubectl-nsenter](https://github.com/towolf/kubectl-nsenter)                       | Simple kubectl plugin to take pod name, SSH onto node and spawn an nsenter shell               | Exec                |
| 26  | [kvaps kubectl-ssh](https://github.com/kvaps/kubectl-ssh)                          | Tiny plugin for connecting to node in the cluster over SSH                                      | Exec                |
| 27  | [kubectl-warp](https://github.com/ernoaapa/kubectl-warp)                           | Kubernetes CLI plugin for syncing and executing local files in Pod on Kubernetes               | Exec                |
| 28  | [kubectl-plugin-ssh-jump](https://github.com/yokawasa/kubectl-plugin-ssh-jump)     | A kubectl plugin to SSH into Kubernetes nodes using a SSH jump host Pod                          | Exec                |
| 29  | [kubectl-texec](https://github.com/TrsNium/kubectl-texec)                          | Attach to the pod matching the label with Tmux                                                | Exec                |
| 30  | [kubectl-dig](https://github.com/sysdiglabs/kubectl-dig)                           | Deep kubernetes visibility from the kubectl                                                     | Visibility          |
| 31  | [kubectl-utility](https://github.com/metrosystems-cpe/kubectl-utility)             | Utility tool for observing k8s resources.                                                        | Visibility          |
| 32  | [kubectl-graph](https://github.com/steveteuber/kubectl-graph)                      | A kubectl plugin to visualize Kubernetes resources and relationships.                                                        | Visibility          |
| 33  | [kubectl-tree](https://github.com/ahmetb/kubectl-tree)                             | A kubectl plugin to browse Kubernetes object hierarchies as a tree                               | Visibility          |
| 34  | [kubectl-topology](https://github.com/bmcustodio/kubectl-topology)                 | A kubectl plugin that provides insight into the topology of a Kubernetes cluster.                | Visibility          |
| 35  | [Pod-Dive](https://github.com/caiobegotti/Pod-Dive)                                 | A kubectl plugin to dive into your Kubernetes nodes pods, and inspect them.               | Visibility          |
| 36  | [kubectl-dashboard](https://github.com/bouk/kubectl-dashboard)                      | Instantly get a Kubernetes dashboard                                                            | Visibility          |
| 37  | [kubelogin](https://github.com/int128/kubelogin)                                    | kubectl plugin for Kubernetes OpenID Connect authentication (kubectl oidc-login)               | Authn/Authz         |
| 38  | [k8s-pixy-auth](https://github.com/auth0/k8s-pixy-auth)                             | k8s plugin to authenticate against an OIDC compatible issuer using PKCE (pixy) flow           | Authn/Authz         |
| 39  | [kubectl-login](https://github.com/sdrozdkov/kubectl-login)                         | Kubectl plugin for re-authenticate into OpenID Connect Provider via CLI                        | Authn/Authz         |
| 40  | [zjj2wry kubectl-login](https://github.com/zjj2wry/kubectl-login)                   | The kubectl plugin is used to login to the kubernetes cluster by oidc authentication.       | Authn/Authz         |
| 41  | [kubectl-pass](https://github.com/rafi/kubectl-pass)                                | kubectl plugin for integration with pass (the standard unix password manager)                  | Authn/Authz         |
| 42  | [kubectl-ssm-secret](https://github.com/pr8kerl/kubectl-ssm-secret)                 | A kubectl plugin to allow import/export of kubernetes secrets to/from AWS SSM Parameter Store path. | Secrets           |
| 43  | [kubectl-decode-secret](https://github.com/brosandilabs/kubectl-decode-secret)      | A kubectl plugin to decode Kubernetes secrets                                             | Secrets             |
| 44  | [kubectl-gopass](https://github.com/gopasspw/kubectl-gopass)                        | Plugin for kubectl to support reading and writing secrets directly from/to gopass          | Secrets             |
| 45  | [kubectl-modify-secret](https://github.com/rajatjindal/kubectl-modify-secret)       | kubectl-modify-secrets allows user to directly modify the secret without worrying about base64 encoding/decoding                                                               | Secrets             |
| 46  | [weibeld kubectl-ctx](https://github.com/weibeld/kubectl-ctx)                       | A kubectl plugin for interactively changing the kubeconfig context                        | Context/Namespace Switching   |
| 47  | [weibeld kubectl-ns](https://github.com/weibeld/kubectl-ns)                       | A kubectl plugin for interactively switching between namespaces in your cluster                  | Context/Namespace Switching   |
| 48  | [kubectl-select-context](https://github.com/stefanm8/kubectl-select-context)        | light kubectl plugin that prompts user to select config context                               | Context/Namespace Switching   |
| 49  | [kubectl-use](https://github.com/kvaps/kubectl-use)                                 | Plugin for simple switch kubernetes contexts and namespaces                                | Context/Namespace Switching   |
| 50  | [kubectx](https://github.com/ahmetb/kubectx)                                        | Switch faster between clusters and namespaces in kubectl https://kubectx.dev                  | Context/Namespace Switching   |
| 51  | [kubectl-ns](https://github.com/postfinance/kubectl-ns)                            | Simple kubectl plugin to display/switch namespaces                                             | Context/Namespace Switching   |
| 52  | [kubectl-use](https://github.com/kvaps/kubectl-use)                                | Plugin for simple switch kubernetes contexts and namespaces                                | Context/Namespace Switching   |
| 53  | [kubectl-switch](https://github.com/yulibaozi/kubectl-switch)                      | Kubernetes multi-cluster command-line management tool                                      | Context/Namespace Switching   |
| 54  | [caas-one kubectl-switch](https://github.com/caas-one/kubectl-switch)              | Kubernetes multi-cluster command-line management tool                                      | Context/Namespace Switching   |
| 55  | [juanvallejo kubectl-ns](https://github.com/juanvallejo/kubectl-ns)              | Quickly view or change the current namespace via kubectl                                        | Context/Namespace Switching   |
| 56  | [km](https://github.com/cststack/km)                                             | EKS MFA kubeconfig management tool. Thin wrapper for kubectl.                                      | Context/Namespace Switching   |
| 57  | [ketall](https://github.com/corneliusweig/ketall)                                  | Like `kubectl get all`, but get really all resources                                          | Resource CRUDs         |
| 58  | [kubectl-grep](https://github.com/guessi/kubectl-grep)                             | Filter Kubernetes resources by matching their names                                    | Resource CRUDs         |
| 59  | [kubectl-all](https://github.com/kajanth/kubectl-all)                               | kubectl plugin to list all resources in given namespace                                        | Resource CRUDs         |
| 60  | [kubectl-watch](https://github.com/lee0c/kubectl-watch)                              | Watches Kubernetes resources                                                            | Resource CRUDs         |
| 61  | [kubectl-custom-cols](https://github.com/webofmars/kubectl-custom-cols)              | a kubectl plugin that help you customize output columns like a boss !                     | Resource CRUDs         |
| 62  | [kubepod](https://github.com/karancode/kubepod)                                     | Search pods faster in kubectl                                                               | Resource CRUDs         |
| 63  | [kubectl-resources](https://github.com/howardjohn/kubectl-resources)                | Plugin to access Kubernetes resource requests, limits, and usage.                         | Resource CRUDs         |
| 64  | [kubectl-free](https://github.com/makocchi-git/kubectl-free)                         | Show various requested resources on Kubernetes nodes                                         | Resource CRUDs         |
| 65  | [kubectl-match-name](https://github.com/gerald1248/kubectl-match-name)               | regex matching for resource names                                                              | Resource CRUDs         |
| 66  | [kubectl-eksporter](https://github.com/Kyrremann/kubectl-eksporter)               | A simple Ruby-script to export k8s resources                                             | Resource CRUDs         |
| 67  | [kube-capacity](https://github.com/robscott/kube-capacity)               | A simple CLI that provides an overview of the resource requests, limits, and utilization in a Kubernetes cluster | Resource CRUDs       |
| 68  | [kubectl-rotate-pods](https://github.com/mousavian/kubectl-rotate-pods)              | kubectl plugin to easily restart all pods of a deployment                                      | Resource CRUDs        |
| 69  | [kubectl-terminate](https://github.com/xcoulon/kubectl-terminate)                    | kubectl-terminate, a kubectl plugin to remove finalizers and finally delete k8s resources  | Resource CRUDs        |
| 70  | [kubectl-extension-versions](https://github.com/GoogleCloudPlatform/kubectl-extension-versions) | Filter Kubernetes resources by matching their names                             | Controller/Operator    |
| 71  | [kudo](https://kudo.dev/docs/cli.html#setup-the-kudo-kubectl-plugin)                 | A kubectl plugin to use [kudo](https://kudo.dev/) via kubectl CLI                         | Controller/Operator    |
| 72  | [ipick](https://github.com/similarweb/kubectl-ipick)                 | A kubectl wrapper for interactive resource selection                   | Controller/Operator    |
| 73  | [kubectl-tmux-logs](https://github.com/brosandilabs/kubectl-tmux-logs)              | A kubectl plugin to display container logs within separate tmux panes                     | Logging                |
| 74  | [kubectl-clogs](https://github.com/ivkalita/kubectl-clogs)                          | kubectl plugin to follow logs of multiple running pods                                         | Logging                |
| 75  | [kubectl-mtail](https://gitlab.com/grzesuav/kubectl-mtail)                          | Kubectl helper to get logs from multiple pods                                                  | Logging                |
| 76  | [kubectl-open-svc-plugin](https://github.com/superbrothers/kubectl-open-svc-plugin) | kubectl open-svc plugin makes services accessible via their ClusterIP from outside your cluster | Uncategorized  |
| 77  | [kubectl-doctor](https://github.com/emirozer/kubectl-doctor)                        | k8s cluster triage plugin - scan your cluster for anomalies (brew doctor equivalent)        | Uncategorized          |
| 78  | [kubectl-view-serviceaccount-kubeconfig-plugin](https://github.com/superbrothers/kubectl-view-serviceaccount-kubeconfig-plugin)              | A kubectl plugin that show a kubeconfig to access the apiserver with a specified serviceaccount.                     | Uncategorized     |
| 79  | [unfork](https://github.com/replicatedhq/unfork)                                    | Kubectl plugin to find forked Helm Charts and other K8s resources and unfork them https://www.unfork.io | Uncategorized       |
| 80  | [kubectl-config-merge](https://github.com/kubedev/kubectl-config-merge)              | A kubectl plugin for merging multiple kubeconfig files. A cli-runtime example.            | Uncategorized          |
| 81  | [konfig](https://github.com/corneliusweig/konfig)                                    | konfig helps to merge, split or import kubeconfig files                                         | Uncategorized       |
| 82  | [kubectlsafe](https://github.com/esin/kubectlsafe)                                   | Safe operations in kubectl with plugin kubectlsafe                                   | Uncategorized          |
| 83  | [kubectl-rainbow](https://github.com/retr0h/kubectl-rainbow)                         | Simple binary to colorize output.                                                             | Uncategorized          |
| 84  | [kubectl-ansible](https://github.com/moshloop/kubectl-ansible)                       | An ansible dynamic inventory plugin for kubernetes cluster nodes                           | Uncategorized          |
| 85  | [kubectl-server-version](https://github.com/bmuschko/kubectl-server-version)         | A kubectl plugin for rendering the Kubernetes server version.                             | Uncategorized          |
| 86  | [kubectl-config-cleanup](https://github.com/b23llc/kubectl-config-cleanup)           | A kubectl plugin for automatically cleaning up your kubeconfig                            | Uncategorized          |
| 87  | [kubectl-gitlab-bootstrap](https://github.com/eddiezane/kubectl-gitlab_bootstrap)    | Quickly add a Kubernetes cluster to a GitLab project                                          | Uncategorized          |
| 88  | [kubectl-captain](https://github.com/alauda/kubectl-captain)                         | kubectl plugin for captain                                                                     | Uncategorized          |
| 89  | [kubectl preflight](https://github.com/replicatedhq/troubleshoot)                    | Preflight Checks and Support Bundles Framework for Kubernetes Applications https://troubleshoot.sh  | Uncategorized          |
| 90  | [kubectl support-bundle](https://github.com/replicatedhq/troubleshoot)               | Preflight Checks and Support Bundles Framework for Kubernetes Applications https://troubleshoot.sh  | Uncategorized          |
| 91  | [kubectl-virt-plugin](https://github.com/kubevirt/kubectl-virt-plugin)               | Holds all scripts to create packages and manifest file required for publishing the virtctl binary as a krew package for kubectl.  | Uncategorized          |
| 92  | [kcf](https://github.com/kubectl-plus/kcf)                                           | A CLI tool providing you with status & configuration of a Kubernetes cluster fleet       | Uncategorized          |
| 93  | [kubepug](https://github.com/rikatz/kubepug)                                         | Kubernetes PreUpGrade (Checker)                                                          | Uncategorized          |
| 94  | [kubectl view-secret](https://github.com/elsesiy/kubectl-view-secret)                                         | Decode Kubernetes secrets                                                      | Secrets |
| 95  | [kubectl-cilium](https://github.com/bmcustodio/kubectl-cilium)                     | A kubectl plugin for interacting with Cilium.                                                    | Networking
| 96  | [kubectl-carbonetes-scan](https://github.com/carbonetes/kubectl-carbonetes-scan)   | Integrates container analysis directly into your cluster. | Container Security |
| 97  | [kubectl-cyclonus](https://github.com/mattfenwick/kubectl-cyclonus)                     | Analyze, explain, and probe network policies.                                                    | Networking |
| 98  | [kubectl-view-webhook](https://github.com/Trendyol/kubectl-view-webhook)           | Visualize your webhook configurations                                                                | Visibility |
| 99  | [kubectl-translate](https://github.com/konveyor/move2kube)           | Helps migrate your app to run on Kubernetes. Generates K8s yamls, Helm chart, Operator, CI/CD pipeline, Kustomize overlays, etc.                                                                | Migration |
| 100 | [kubectl-datree](https://github.com/datreeio/kubectl-datree) | Scan resources within your cluster for misconfigurations | Misconfiguration Detection |
| 101 | [kubectl-irsa](https://github.com/WoodProgrammer/kubectl-irsa) | Check the IAM capabilities of the serviceaccounts via AWS PolicySimulator | Security |
| 102 | [kubectl-dumpy](https://github.com/larryTheSlap/dumpy) | Performs tcpdump captures on resources | Networking |

### Collection of kubectl plugins

* [collection of kubectl plugins](https://github.com/jordanwilson230/kubectl-plugins) - A Collection of Plugins for kubectl Integration (context switching, ssh / exec as any user, etc).

* [kubectl-extras mini plugins](https://github.com/ahmetb/kubectl-extras) - A collection of mini plugins for kubectl.

* [collection - kubectl plugins](https://github.com/thecloudnatives/kubectl-plugins) - A list of plugins that enhance the kubectl CLI

* [collection - kubectl plugins](https://github.com/thobiast/kubectl-plugins) - It is a set of kubectl plugins.

* [collection - kubectl plugins](https://github.com/ripta/kubectl-plugins) - These be collection of kubectl plugins!

* [kubectl-everything](https://github.com/PeterGrace/kubectl-everything) - Various kubectl plugins to make life easier
