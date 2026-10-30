# Uniview Kube Hub

Uniview Kube Hub is a light-weight multi-tenant mulit-cluster Kubernetes management platform that enables enterprise to share Kubernetes infrastures within the organization or to external clients easily and consistently.
The current repo is for public pullable artifacts and utilities for successful deploy, manage, and customize of Uniview Kube Hub.  It complements the official documentation of Uniview official website below. 

For further details, refer to: 
- Product page: https://www.computingstack.com/uniview-kube-hub
- Documentation: https://www.computingstack.com/docs/docs/kubehub/


## 🚀 Why Uniview Kube Hub

**Uniview’s functionality is unique**, yet it delivers the same secure and effective enterprise multi-tenancy as vCluster and Capsule, enabling teams or external clients to safely share a cluster. Uniview also manages anywhere from a few to hundreds of clusters via a massive API Broker. This allows users to sign in to a single platform to access multiple clusters—similar to Rancher Prime or Teleport. 

For effective metering and billing from a single entry point, Uniview implements features akin to OpenCost and KubeCost. Additionally, Uniview integrates Cluster API (CAPI) as a built-in console, allowing users to provision clusters over bare-metal, AWS, GCP, and other providers. Ultimately, Uniview is a distinct, comprehensive solution designed to tackle the most pressing infrastructure challenges for the enterprise.

---

## 🔁 Alternatives Breakdown

### Uniview Kube Hub vs. vCluster
If you like how vCluster helps share a cluster within an organization, but worry that its bloated in-cluster objects make production workloads hard to maintain, Uniview Kube Hub is the ideal alternative. 
* **Zero Overhead:** Requires no binaries or pods to run inside your cluster.
* **Lightweight:** Relies only on a fraction of static tenant policies.
* **Isolate Workloads:** Seamlessly shares namespaces and enables dedicated nodes to eliminate noisy-neighbour issues.
* **Cluster-Level Access:** For users requiring cluster-level operators, Uniview can easily share an entire cluster as an admin or member instead of restricting access to a namespace, perfectly meeting practical production requirements.

### Uniview Kube Hub vs. Rancher Prime
If you like how Rancher Prime manages hundreds of clusters through a single broker and unified sign-in, but worry about its massive overhead and complexity, Uniview is the perfect alternative. Rancher Prime was originally designed for an end-to-end ecosystem tailored to its own Kubernetes distribution (RKE2) and provisioning system. 
* **Bring Your Own Cluster (BYOC):** If you are concerned that your custom provisioning engine—whether CAPI or another tool—cannot be easily integrated into Rancher Prime, Uniview fits right in. 
* **Ecosystem Friendly:** It is not designed to replace your infrastructure; instead, it seamlessly complements your existing ecosystem.
* **True Multi-Tenancy:** Uniview’s access control is far more effective, scalable, and repeatable as a Tenant-as-a-Service model compared to Rancher Prime, which relies on internal tenancy across separate target clusters and struggles to scale to a huge user base.

### Uniview Kube Hub vs. Teleport
If you like how Teleport manages access to multiple clusters with a single sign-in and a decoupled architecture, but worry that Teleport’s short-lived access certificates may break standard ecosystem workflows—such as machine-based authentication—Uniview Kube Hub is an excellent alternative. 
* **Built Natively for K8s:** If you feel Teleport lacks a true platform experience for user management, cost optimization, and service support, Uniview fills that gap. 
* **Hybrid Access:** Natively designed for Kubernetes to securely satisfy access requirements for both humans and machines across hundreds of clusters.

### Uniview Kube Hub vs. Capsule
If you like how Capsule implements tenant grouping and uses an API proxy to route and vet user requests, but worry that its complex `kubectl` setup alters native Kubernetes behavior, Uniview Kube Hub is the best alternative. You may also be concerned that Capsule remains a CNCF Sandbox project after many years, introducing investment uncertainty. 
* **External Management:** Uniview delivers the same tenant grouping capabilities but handles them externally outside of the cluster. 
* **Native Experience:** It provides a generic, upstream Kubernetes user experience with minimal modifications, making the platform layer completely transparent to the user. 
* **Production-Proven Stack:** Uniview relies exclusively on CNCF-graduated artifacts and proven, primitive technologies rather than unproven sandbox techniques.

---

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






