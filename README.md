# Uniview Kube Hub

Uniview Kube Hub is a light-weight multi-tenant mulit-cluster Kubernetes management platform that enables enterprise to share Kubernetes infrastures within the organization or to external clients easily and consistently.
The current repo is for public pullable artifacts and utilities for successful deploy, manage, and customize of Uniview Kube Hub.  It complements the official documentation of Uniview official website below. 

For further details, refer to: 
- Product page: https://www.computingstack.com/uniview-kube-hub
- Documentation: https://www.computingstack.com/docs/docs/kubehub/

## 🚀 Why Uniview Kube Hub

If you like how **vCluster** helps share a cluster within an organization, but worry that its **bloated in-cluster objects** make production workloads hard to maintain, **Uniview Kube Hub** is the ideal alternative. Uniview introduces **zero overhead**—requiring **no binaries or pods to run**—and relies only on a fraction of static tenant policies. It seamlessly shares namespaces and enables **dedicated nodes** to eliminate **noisy-neighbour** issues. For users requiring **cluster-level operators**, Uniview can easily share an entire cluster as an admin or member instead of restricting access to a namespace, perfectly meeting practical production requirements.

If you like how **Rancher Prime** manages hundreds of clusters through a single broker and unified sign-in, but worry about its **massive overhead and complexity**, Uniview is the perfect alternative. Rancher Prime was originally designed for an end-to-end ecosystem tailored to its own Kubernetes distribution (**RKE2**) and provisioning system. If you are concerned that your custom provisioning engine—whether **CAPI** or another tool—cannot be easily integrated into Rancher Prime, Uniview fits right in. Uniview Kube Hub works with any **"Bring Your Own Cluster" (BYOC)** model and any existing provisioning engine. It is not designed to replace your infrastructure; instead, it seamlessly complements your existing ecosystem. Furthermore, you will find Uniview’s access control to be far more effective, scalable, and repeatable as a **Tenant-as-a-Service** model compared to Rancher Prime, which relies on **internal tenancy** across separate target clusters and struggles to scale to a huge user base.

If you like how **Teleport** manages access to multiple clusters with a single sign-in and a decoupled architecture, but worry that Teleport’s **short-lived access certificates** may break standard ecosystem workflows—such as **machine-based authentication**—Uniview Kube Hub is an excellent alternative. If you also feel Teleport lacks a true platform experience for user management, cost optimization, and service support, Uniview fills that gap. It is designed **natively for Kubernetes** and securely satisfies access requirements for both **humans and machines** across hundreds of clusters.

If you like how **Capsule** implements tenant grouping and uses an API proxy to route and vet user requests, but worry that its **complex kubectl setup** alters native Kubernetes behavior, Uniview Kube Hub is the best alternative. You may also be concerned that Capsule remains a **CNCF Sandbox** project after many years, introducing investment uncertainty. Uniview delivers the same tenant grouping capabilities but handles them **externally outside of the cluster**. It provides a generic, **upstream Kubernetes user experience** with minimal modifications, making the platform layer completely transparent to the user. Uniview relies exclusively on **CNCF-graduated artifacts** and proven, primitive technologies rather than unproven sandbox techniques.

If you like the enterprise-grade management provided by **Rancher Prime** or the **OpenShift OIDC** management framework, but realize that they are limited in how they balance granular namespace management with global access, Uniview is the perfect alternative. Uniview allows you to manage infrastructure cleanly at **both the cluster level and the namespace level** simultaneously. For shared clusters, **namespace-level resource access control** in Uniview is a first-class feature, delivering identical elite management capabilities across any boundary you define.
## Quick Architecture Conception of Uniview Kube Hub
The quick architecture view of Uniview Kube Hub:

<p align="center">
  <img src="/images/uniview-framework.svg" alt="Uniview Framework" max-width="450">
</p>



## 🎯 Addressing Enterprise Flaws

Uniview provides matching capabilities while bypassing the flaws of legacy tools:

> [!TIP]
> ### 💡 Quick Comparison Table
> | Legacy Challenge | The Uniview Solution |
> | :--- | :--- |
> | **Bloated in-cluster objects** *(vCluster/Capsule)* | Uniview moves them entirely outside the cluster. |
> | **Complicated Kubectl CLI setup** *(Capsule/Rancher)* | Uniview remains natively identical to upstream Kubernetes. |
> | **New services (like KubeVirt) blocked** *(vCluster)* | Uniview uses no synchronization mechanisms that could block them. |
> | **Missing multi-cluster support** *(Capsule/vCluster)* | Uniview supports multi-cluster natively. |
> | **Abstract or manual tenant onboarding** *(Rancher Auth)* | Uniview simplifies onboarding to just one single step. |
> | **Thin, feature-limited tooling** *(Competitors)* | Uniview is built from the ground up to be truly enterprise-grade. |
> | **Insecure KCP integration with subject cluster** | Uniview is reinforced using a robust OIDC mechanism. |






