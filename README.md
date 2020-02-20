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

* [Extending kubectl with plugins](https://kubernetes.io/docs/tasks/extend-kubectl/kubectl-plugins/)
* [Write your own kubectl subcommands](https://ahmet.im/blog/kubectl-plugins/)
* [Manage Kubernetes Plugins with Krew](https://thepracticalsysadmin.com/manage-kubernetes-plugins-with-krew/)
* [Boosting Your Kubectl Productivity](https://learnk8s.io/blog/kubectl-productivity/)

## kubectl Plugins
* [kubectx](https://github.com/ahmetb/kubectx) - Switch faster between clusters and namespaces in kubectl https://kubectx.dev

* [kubectl-debug](https://github.com/aylei/kubectl-debug) - Debug your pod by a new container with every troubleshooting tools pre-installed

* [kubectl-trace](https://github.com/iovisor/kubectl-trace) - Schedule bpftrace programs on your kubernetes cluster using the kubectl

* [ksniff](https://github.com/eldadru/ksniff) - Kubectl plugin to ease sniffing on kubernetes pods using tcpdump and wireshark

* [rakkess](https://github.com/corneliusweig/rakkess) - Review Access - kubectl plugin to show an access matrix for k8s server resources

* [kubectl-dig](https://github.com/sysdiglabs/kubectl-dig) - Deep kubernetes visibility from the kubectl

* [kubectl-doctor](https://github.com/emirozer/kubectl-doctor) - k8s cluster triage plugin - scan your cluster for anomalies (brew doctor equivalent)

* [kubectl-warp](https://github.com/ernoaapa/kubectl-warp) - Kubernetes CLI plugin for syncing and executing local files in Pod on Kubernetes

* [kubelogin](https://github.com/int128/kubelogin) - kubectl plugin for Kubernetes OpenID Connect authentication (kubectl oidc-login)

* [kubectl-sudo](https://github.com/postfinance/kubectl-sudo) - Run kubernetes commands with the security privileges of another user

* [kubectl-cssh](https://github.com/containership/kubectl-cssh) - A kubectl plugin to ssh into Kubernetes nodes within separate tmux panes

* [ketall](https://github.com/corneliusweig/ketall) - Like `kubectl get all`, but get really all resources

* [kubectl-open-svc-plugin](https://github.com/superbrothers/kubectl-open-svc-plugin) - kubectl open-svc plugin makes services accessible via their ClusterIP from outside your cluster

* [kubectl-capture](https://github.com/sysdiglabs/kubectl-capture) - A kubectl plugin which triggers a Sysdig capture https://sysdig.com/opensource/inspect/

* [kubectl-grep](https://github.com/guessi/kubectl-grep) - Filter Kubernetes resources by matching their names

* [kubectl-tmux-logs](https://github.com/brosandilabs/kubectl-tmux-logs) - A kubectl plugin to display container logs within separate tmux panes

* [kubectl-plugin-ssh-jump](https://github.com/yokawasa/kubectl-plugin-ssh-jump) - A kubectl plugin to SSH into Kubernetes nodes using a SSH jump host Pod

* [kubectl-view-serviceaccount-kubeconfig-plugin](https://github.com/superbrothers/kubectl-view-serviceaccount-kubeconfig-plugin) - A kubectl plugin that show a kubeconfig to access the apiserver with a specified serviceaccount.

* [outdated](https://github.com/replicatedhq/outdated) - Find and report outdated images running in a Kubernetes cluster

* [kubectl-ctx](https://github.com/postfinance/kubectl-ctx) - Simple kubectl plugin to display/switch contexts

* [kubectl-extension-versions](https://github.com/GoogleCloudPlatform/kubectl-extension-versions) - kubectl plugin to print versions of well-known third-party controllers/operators installed in a cluster

* [kubectl-enter](https://github.com/kvaps/kubectl-enter) - Exec into node via kubectl

* [ksort](https://github.com/superbrothers/ksort) - Sort manifest files in a proper order by Kind

* [kubectl-ns](https://github.com/postfinance/kubectl-ns) - Simple kubectl plugin to display/switch namespaces

* [k8s-pixy-auth](https://github.com/auth0/k8s-pixy-auth) - k8s plugin to authenticate against an OIDC compatible issuer using PKCE (pixy) flow

* [unfork](https://github.com/replicatedhq/unfork) - Kubectl plugin to find forked Helm Charts and other K8s resources and unfork them https://www.unfork.io

* [kubectl-config-merge](https://github.com/kubedev/kubectl-config-merge) - A kubectl plugin for merging multiple kubeconfig files. A cli-runtime example.

* [weibeld kubectl-ctx](https://github.com/weibeld/kubectl-ctx) - A kubectl plugin for interactively changing the kubeconfig context

* [kubectl-switch](https://github.com/yulibaozi/kubectl-switch) - Kubernetes multi-cluster command-line management tool

* [kubectl-iexec](https://github.com/gabeduke/kubectl-iexec) - Kubectl plugin to interactively exec into a pod

* [kubectl-dashboard](https://github.com/bouk/kubectl-dashboard) - Instantly get a Kubernetes dashboard

* [kubectl-watch](https://github.com/lee0c/kubectl-watch) - Watches Kubernetes resources

* [konfig](https://github.com/corneliusweig/konfig) - konfig helps to merge, split or import kubeconfig files

* [kubectl-login](https://github.com/sdrozdkov/kubectl-login) - Kubectl plugin for re-authenticate into OpenID Connect Provider via CLI

* [kubectl-free](https://github.com/makocchi-git/kubectl-free) - Show various requested resources on Kubernetes nodes

* [kubectl-ssh](https://github.com/IuryAlves/kubectl-ssh) - A kubectl plugin to ssh into a pod's node

* [weibeld kubectl-ns](https://github.com/weibeld/kubectl-ns) - A kubectl plugin for interactively switching between namespaces in your cluster

* [kubectl-kcn](https://github.com/marjamis/kubectl-kcn) - A script and kubectl plugin which makes it easier to ssh into nodes within your cluster.

* [kubectlsafe](https://github.com/esin/kubectlsafe) - Safe operations in kubectl with plugin kubectlsafe

* [kubectl-rainbow](https://github.com/retr0h/kubectl-rainbow) - Simple binary to colorize output.

* [kubepod](https://github.com/karancode/kubepod) - Search pods faster in kubectl

* [kubectl-all](https://github.com/kajanth/kubectl-all) - kubectl plugin to list all resources in given namespace

* [kubectl-swiftnp](https://github.com/bmuschko/kubectl-swiftnp) - A kubectl plugin for rendering details of Network Policies.

* [kubectl-plugin-pvc](https://github.com/fabiand/kubectl-plugin-pvc) - A simple kubectl binary plugin for PVC operations

* [kubectl-pass](https://github.com/rafi/kubectl-pass) - kubectl plugin for integration with pass (the standard unix password manager)

* [kubectl-clogs](https://github.com/ivkalita/kubectl-clogs) - kubectl plugin to follow logs of multiple running pods

* [caas-one kubectl-switch](https://github.com/caas-one/kubectl-switch) - Kubernetes multi-cluster command-line management tool

* [kubectl-custom-cols](https://github.com/webofmars/kubectl-custom-cols) - a kubectl plugin that help you customize output columns like a boss !

* [kubectl-texec](https://github.com/TrsNium/kubectl-texec) - Attach to the pod matching the label with Tmux

* [duyguserbest kubectl-iexec](https://github.com/duyguserbest/kubectl-iexec) - kubectl plugin to simplify interactive exec command.

* [juanvallejo kubectl-ns](https://github.com/juanvallejo/kubectl-ns) - Quickly view or change the current namespace via kubectl.

* [kubectl-server-version](https://github.com/bmuschko/kubectl-server-version) - A kubectl plugin for rendering the Kubernetes server version.

* [zjj2wry kubectl-login](https://github.com/zjj2wry/kubectl-login) - The kubectl plugin is used to login to the kubernetes cluster by oidc authentication.

* [kubectl-ansible](https://github.com/moshloop/kubectl-ansible) - An ansible dynamic inventory plugin for kubernetes cluster nodes

* [km](https://github.com/cststack/km) - EKS MFA kubeconfig management tool. Thin wrapper for kubectl.

* [kubectl-rotate-pods](https://github.com/mousavian/kubectl-rotate-pods) - kubectl plugin to easily restart all pods of a deployment

* [kubectl-resources](https://github.com/howardjohn/kubectl-resources) - Plugin to access Kubernetes resource requests, limits, and usage.

* [kubectl-config-cleanup](https://github.com/b23llc/kubectl-config-cleanup) - A kubectl plugin for automatically cleaning up your kubeconfig

* [kubectl-match-name](https://github.com/gerald1248/kubectl-match-name) - regex matching for resource names

* [kubectl-exec-all](https://github.com/jpdasma/kubectl-exec-all) - kubectl plugin to execute a command in all running pods of a resource (daemonset, deployment, statefulset, etc)

* [kubectl-select-context](https://github.com/stefanm8/kubectl-select-context) - light kubectl plugin that prompts user to select config context

* [kubectl-gitlab-bootstrap](https://github.com/eddiezane/kubectl-gitlab_bootstrap) - Quickly add a Kubernetes cluster to a GitLab project

* [kubectl-ssm-secret](https://github.com/pr8kerl/kubectl-ssm-secret) - A kubectl plugin to allow import/export of kubernetes secrets to/from AWS SSM Parameter Store path.

* [kubectl-dfi](https://github.com/makocchi-git/kubectl-dfi) - List and show disk resources of images on Kubernetes nodes.

* [kubectl-decode-secret](https://github.com/brosandilabs/kubectl-decode-secret) - A kubectl plugin to decode Kubernetes secrets

* [kubectl-use](https://github.com/kvaps/kubectl-use) - Plugin for simple switch kubernetes contexts and namespaces

* [kubectl-nsenter](https://github.com/towolf/kubectl-nsenter) - Simple kubectl plugin to take pod name, SSH onto node and spawn an nsenter shell

* [kvaps kubectl-ssh](https://github.com/kvaps/kubectl-ssh) - Tiny plugin for connecting to node in the cluster over SSH

* [kubectl-lint](https://github.com/SethCurry/kubectl-lint) - A kubectl plugin to perform linting

* [kubectl-utility](https://github.com/metrosystems-cpe/kubectl-utility) - Utility tool for observing k8s resources.

* [kubectl-captain](https://github.com/alauda/kubectl-captain) - kubectl plugin for captain

* [kubectl-unbound-pvc](https://github.com/ishantanu/kubectl-unbound-pvc) - A kubectl plugin to see PVCs which are not in "Bound" state

* [kudo](https://kudo.dev/docs/cli.html#setup-the-kudo-kubectl-plugin) - A kubectl plugin to use [kudo](https://kudo.dev/) via kubectl CLI

* [kubectl-tree](https://github.com/ahmetb/kubectl-tree) - A kubectl plugin to browse Kubernetes object hierarchies as a tree

* [kubectl-graph](https://github.com/steveteuber/kubectl-graph) - A kubectl plugin to visualize Kubernetes resources and relationships.

* [kubectl-modify-secret](https://github.com/rajatjindal/kubectl-modify-secret) - kubectl-modify-secrets allows user to directly modify the secret without worrying about base64 encoding/decoding

* [kubectl preflight](https://github.com/replicatedhq/troubleshoot) - Preflight Checks and Support Bundles Framework for Kubernetes Applications https://troubleshoot.sh

* [kubectl support-bundle](https://github.com/replicatedhq/troubleshoot) - Preflight Checks and Support Bundles Framework for Kubernetes Applications https://troubleshoot.sh

* [kube-profefe](https://github.com/profefe/kube-profefe) - continuous profiling made easy in Kubernetes with profefe

* [kubectl-who-can](https://github.com/aquasecurity/kubectl-who-can) - Show who has RBAC permissions to perform actions on different resources in Kubernetes

* [kubectl-virt-plugin](https://github.com/kubevirt/kubectl-virt-plugin) - Holds all scripts to create packages and manifest file required for publishing the virtctl binary as a krew package for kubectl.

* [kubectl-topology](https://github.com/bmcstdio/kubectl-topology) - Provides insight into the topology of a Kubernetes cluster.

* [kube-capacity](https://github.com/robscott/kube-capacity) - A simple CLI that provides an overview of the resource requests, limits, and utilization in a Kubernetes cluster

* [kubectl-neat](https://github.com/itaysk/kubectl-neat) - Clean up Kuberntes yaml and json output to make it readable

* [kubectl-mtail](https://gitlab.com/grzesuav/kubectl-mtail) - Kubectl helper to get logs from multiple pods

* [kubectl-kubesec](https://github.com/controlplaneio/kubectl-kubesec) - Security risk analysis for Kubernetes resources https://kubesec.io

* [kubectl-gopass](https://github.com/gopasspw/kubectl-gopass) - Plugin for kubectl to support reading and writing secrets directly from/to gopass

* [kubectl-eksporter](https://github.com/Kyrremann/kubectl-eksporter) - A simple Ruby-script to export k8s resources

* [kubectl-df-pv](https://github.com/yashbhutwala/kubectl-df-pv) - kubectl plugin - giving admins df (disk free) like utility for persistent volumes

* [kcf](https://github.com/kubectl-plus/kcf) - A CLI tool providing you with status & configuration of a Kubernetes cluster fleet

* [Pod-Dive](https://github.com/caiobegotti/Pod-Dive) - A kubectl plugin to dive into your Kubernetes nodes pods, and inspect them.
 
### Collection of kubectl plugins

* [collection of kubectl plugins](https://github.com/jordanwilson230/kubectl-plugins) - A Collection of Plugins for kubectl Integration (context switching, ssh / exec as any user, etc).

* [kubectl-extras mini plugins](https://github.com/ahmetb/kubectl-extras) - A collection of mini plugins for kubectl.

* [collection - kubectl plugins](https://github.com/thecloudnatives/kubectl-plugins) - A list of plugins that enhance the kubectl CLI

* [collection - kubectl plugins](https://github.com/thobiast/kubectl-plugins) - It is a set of kubectl plugins.

* [collection - kubectl plugins](https://github.com/ripta/kubectl-plugins) - These be collection of kubectl plugins!

