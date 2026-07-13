---
api_specs:
- filename: azure-quantum-data-plane-openapi.json
  format: json
  label: Azure Quantum Workspace Data-Plane API
  slug: azure-quantum-workspace-data-plane
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-quantum/refs/heads/main/openapi/azure-quantum-data-plane-openapi.json
- filename: azure-quantum-resource-manager-openapi.json
  format: json
  label: Azure Quantum Resource Manager API
  slug: azure-quantum-resource-manager
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-quantum/refs/heads/main/openapi/azure-quantum-resource-manager-openapi.json
description: ''
domains:
- caa:
  - 0 contactemail "caarecordaware@microsoft.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: microsoft.com
  spf: true
hosts:
- cert_expires: Nov  1 16:12:48 2026 GMT
  host: quantum.microsoft.com
  hsts: true
  hsts_max_age: 31557600
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 24 22:04:48 2026 GMT
  host: azure.microsoft.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 11 02:26:09 2026 GMT
  host: learn.microsoft.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Microsoft Quantum Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Microsoft Azure Quantum, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Microsoft Azure Quantum
provider_slug: microsoft-quantum
slug: microsoft-quantum-domain-security
source_filename: microsoft-quantum-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: quantum.microsoft.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  1 16:12:48 2026 GMT\n  hsts: true\n  hsts_max_age: 31557600\n- host: azure.microsoft.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 24 22:04:48 2026 GMT\n  hsts: null\n- host: learn.microsoft.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 11 02:26:09 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: microsoft.com\n  dnssec: false\n  caa:\n  - 0 contactemail \"caarecordaware@microsoft.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/microsoft-quantum/refs/heads/main/security/microsoft-quantum-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Quantum
- Quantum Computing
- Azure
- Microsoft
- Q#
- QDK
- Resource Estimation
- IonQ
- Quantinuum
- Pasqal
- Rigetti
- Hybrid Quantum
- Fault Tolerance
---
