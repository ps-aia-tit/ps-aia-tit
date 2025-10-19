# 🌐 OpenShift Microservices Architecture — Enterprise-Grade, Cloud-Native Design

## 🔥 Overview

This repository showcases a reimagined microservices architecture originally deployed on Pivotal Cloud Foundry (PCF), now fully adapted for **Red Hat OpenShift**. It reflects a strategic modernization journey, integrating Kubernetes-native constructs, service mesh, and CI/CD automation while preserving modular clarity and enterprise integration patterns.

Designed by **Purnendu Shankar**, Senior Java Technical Lead specializing in hybrid Kafka–IBM MQ flows, cloud-native modernization, and recruiter-facing documentation.

---

## 🧱 Architecture Highlights

- **Platform**: Red Hat OpenShift (Kubernetes)
- **API Management**: 3scale API Gateway / Istio Ingress
- **Authentication**: Keycloak / Red Hat SSO
- **Service Mesh**: Istio + Kiali + Jaeger
- **CI/CD**: OpenShift Pipelines (Tekton) + ArgoCD
- **Observability**: Prometheus, Grafana, EFK Stack
- **Backend Integration**: DB2, MSSQL, IBM MQ (Operator-based)
- **Deployment Strategy**: GitOps, Declarative YAML, Modular Helm Charts

---

## 📌 Key Components

| Layer              | Technology Stack                                      |
|--------------------|-------------------------------------------------------|
| Ingress            | OpenShift Route / Istio Gateway                       |
| API Gateway        | 3scale / Envoy Proxy                                  |
| AuthN/AuthZ        | Keycloak / RH-SSO                                     |
| Service Discovery  | Istio + Kiali + Jaeger                                |
| Microservices      | Spring Boot / Quarkus Pods with ConfigMaps & Secrets |
| Backend            | DB2, MSSQL, IBM MQ via Operators                      |
| CI/CD              | Tekton Pipelines + ArgoCD                             |
| Logging & Metrics  | Prometheus, Grafana, Fluentd, Elasticsearch, Kibana  |

---

## 📊 Architecture Diagram

> 📌 *Diagram coming soon: includes ingress, gateway, service mesh, microservices, and backend integrations.*

---

## 🚀 Deployment Flow

```plaintext
Client → Route/Ingress → API Gateway → Microservices → Service Mesh → Backend (DB/MQ)
        ↘ Auth via Keycloak/RH-SSO
        ↘ Observability via Prometheus + Grafana + Jaeger
        ↘ CI/CD via Tekton + ArgoCD
