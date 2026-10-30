# Uniview Kube Hub

Uniview Kube Hub is a light-weight multi-tenant mulit-cluster Kubernetes management platform that enables enterprise to share Kubernetes infrastures within the organization or to external clients easily and consistently.
The current repo is for public pullable artifacts and utilities for successful deploy, manage, and customize of Uniview Kube Hub.  It complements the official documentation of Uniview official website below. 

For further details, refer to: 
- Product page: https://www.computingstack.com/uniview-kube-hub
- Documentation: https://www.computingstack.com/docs/docs/kubehub/


## Why Uniview Kub Hub

Uniview functionality wise, is unique, but from functionality wise, it implements the same multi-tenancy for enterprise to securely and effectively share a cluster to teams or external clients, as vCluster and Capsule. Uniview also manages from many up to hundreds clusters, providing a massive API Broker, so that users can sign in one platform to access many clusters, as Rancher Prime, Teleport. Uniview implements function as OpenCost, KubeCost etc, to effectively manage metering and billing from the same entry. Uniview integrates CAPI cluster, as the CAPI console, user literally can provision cluster over Bare-metal,  AWS, GCP and others. 
Uniview is unique and more comprehensively tackling the pressing issues for enterprise. 


If you like vCluster that helps share a cluster within an organization, but worry vCluster is over-bloated objects within cluster and that is very hard to maintain for prod workload manageability, Uniview Kube Hub is an ideal alternative. Uniview introduces zero overhead, no binary, no pod to run, only a fraction static tenant policy, and it can share namespace and enable dedicated node to avoid noising etc. For user who requires cluster level operators, Uniview can easily share a while cluster as admin or member, instead of a namespace to meet the practical requirements.

If you like how Rancher Prime is managing hundreds of clusters, one big broker, one sign-in, but worry Rancher Prime has huge overhead and complexity, as it was originated for end-to-end ecosystem, for Rancher RKE2 its own kubernetes distro, provisioning oriented system, if you worry your own-provisioning system either CAPI, or by other engine, can't be easily integrated with Rancher Prime, Uniview is a perfect alternative choice in such sitations. Uniview Kube Hub works with any Bring Your Own Clusters, any your own provisioning engine. It is not designed to replace, instead, it seamlessly works with your existing ecosystem. In the meanwhile, you will find Uniview Access Control can be way effective, scalable, repeatable and tenant as a service, to compare with Rancher Prime which is rather internal tenant, separate target cluster and Prime make it hard to scale to huge user base.

If you like how Teleport manages access to many clusters by one user, one sign in, and decoupled architecture, but worry Teleport short lived access certificate may not work with general ecosystem, such as machine based authentication, and worry it has no a sense of platform by user management, cost and service support, then Uniview Kube Hub is good alternative, that it's designed for Kubernetes genetically, and well meet access by human and as well by machine to many up to hundreds of cluster securely

If you like Capsule on how it how implements tenant grouping, API proxy to route and vet user requests, but worry it changed the behaviror of Kubernetes by kubectl setup, not user friendly, and Capsule still CNCF sandbox project after many years with huge investment uncertainty, Uniview Kube Hub is the best alternative. It does the same on tenant grouping, but externally out side of cluster, and its user experience is generic as upstream kuberentes is with minimal modification that user is never aware. Uniview uses only the CNCF granduated artifacts and very primitive technology, no sandbox technique et all. 

If you like Spector and Platform 9 platform that get Kubernetes enterprise grade supported, but worry there is huge maintainance debut, and in most of the case, managed services have to be bound, Uniview can be the best alternative. Uniview is maintainnance free, decoupled architecture and mature architecture ensure small team is good enough to confidently manage a large cluster. Uniview is not a ecosystem or service forced, instead its goal is to complement whatever in your ecosystem. Uniview Kube Hub is only software core piences that expects to work with your own such as CAPI engine, prometheus, different cloud providers etc. 


Uniview provides matching capabilities while bypassing their flaws. For instance: Worry about bloated objects within cluster from vCluster or Capsule that is hard to maintain? Uniview has them outside of cluster! Worry about Kubectl CLI setup complicated experience from Capsule/Rancher? Uniview remains natively the same. Worry a new service like KubeVirt is not supported by multi-tenant layer such as vCluster? Uniview has no sync mechanism to block them! Concern multi-cluster is not supported by Capsule or vCluster? Uniview supports it natively! Concern tenant onboarding is abstract or manual on Rancher Auth? Uniview is just one step! Worry they are thin and function-limited? Uniview is true enterprise-grade! KCP integrated with subject cluster not secure? Uniview is reinforced with our OIDC mechanism.
