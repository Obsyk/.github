<picture>
  <source media="(prefers-color-scheme: dark)" srcset="https://obsyk.ai/assets/logo-white.svg">
  <source media="(prefers-color-scheme: light)" srcset="https://obsyk.ai/assets/logo.svg">
  <img alt="Obsyk" src="https://obsyk.ai/assets/logo.svg" width="200">
</picture>

# See Everything Running in Your Kubernetes Clusters

**Deploy in 2 minutes. No agents to configure. Instant visibility into pods, services, RBAC, and more.**

[![Website](https://img.shields.io/badge/Website-obsyk.ai-0066FF?style=flat-square)](https://obsyk.ai)
[![Documentation](https://img.shields.io/badge/Docs-docs.obsyk.ai-0066FF?style=flat-square)](https://docs.obsyk.ai)
[![Platform](https://img.shields.io/badge/Platform-app.obsyk.ai-0066FF?style=flat-square)](https://app.obsyk.ai)

---

## The Problem

Security teams deploy workloads but have **no visibility** into what's running, what changed, and whether it's secure. Kubernetes complexity makes it nearly impossible to answer simple questions:

- What's actually running in production right now?
- Who has access to what across all clusters?
- Did that deployment change anything unexpected?

## The Solution

Obsyk gives you **complete visibility** across all your Kubernetes clusters in a unified dashboard. See pods, services, deployments, RBAC permissions, and more—without the complexity.

<table>
<tr>
<td width="33%" align="center">
<h3>Full Visibility</h3>
<p>See all resources across all clusters. Pods, services, deployments, RBAC—everything in one place.</p>
</td>
<td width="33%" align="center">
<h3>Security Posture</h3>
<p>Understand your RBAC exposure. See who has access to what across your entire infrastructure.</p>
</td>
<td width="33%" align="center">
<h3>2-Minute Setup</h3>
<p>Deploy our lightweight operator with a single Helm command. Read-only access, signed images.</p>
</td>
</tr>
</table>

---

## Quick Start

### 1. Sign up at [app.obsyk.ai](https://app.obsyk.ai)

### 2. Install the operator

```bash
helm repo add obsyk https://obsyk.github.io/obsyk-operator
helm repo update

helm install obsyk-operator obsyk/obsyk-operator \
  --namespace obsyk-system --create-namespace \
  --set agent.clusterName="my-cluster"
```

### 3. View your clusters

Your infrastructure appears in the dashboard within seconds. No configuration required.

---

## Enterprise-Grade Security

<table>
<tr>
<td>:lock: <strong>Read-Only Access</strong></td>
<td>The operator only watches resources—no write permissions, no risk.</td>
</tr>
<tr>
<td>:closed_lock_with_key: <strong>Signed Images</strong></td>
<td>All container images are signed with Sigstore and include SLSA provenance.</td>
</tr>
<tr>
<td>:shield: <strong>No Secrets Transmitted</strong></td>
<td>ConfigMap and Secret data values never leave your cluster.</td>
</tr>
<tr>
<td>:page_facing_up: <strong>Auditable</strong></td>
<td>Full SBOM (Software Bill of Materials) included with every release.</td>
</tr>
</table>

---

## Open Source

| Repository | Description |
|------------|-------------|
| [obsyk-operator](https://github.com/Obsyk/obsyk-operator) | Kubernetes operator that connects your cluster to Obsyk |
| [docs](https://github.com/Obsyk/docs) | User documentation and guides |

---

## Resources

- **Website**: [obsyk.ai](https://obsyk.ai)
- **Documentation**: [docs.obsyk.ai](https://docs.obsyk.ai)
- **Platform**: [app.obsyk.ai](https://app.obsyk.ai)
- **API Reference**: [developers.obsyk.ai](https://developers.obsyk.ai)

---

<p align="center">
<strong>Ready to see your Kubernetes clusters?</strong><br>
<a href="https://app.obsyk.ai">Get Started Free</a> — No credit card required
</p>
