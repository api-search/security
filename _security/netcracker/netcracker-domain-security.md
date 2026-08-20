---
api_specs:
- filename: netcracker-qubership-apihub-registry-openapi.yml
  format: yaml
  label: Qubership APIHUB Registry API
  slug: qubership-apihub-registry-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/netcracker/refs/heads/main/openapi/netcracker-qubership-apihub-registry-openapi.yml
- filename: netcracker-qubership-apihub-admin-openapi.yml
  format: yaml
  label: Qubership APIHUB System Administrators API
  slug: qubership-apihub-admin-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/netcracker/refs/heads/main/openapi/netcracker-qubership-apihub-admin-openapi.yml
- filename: netcracker-qubership-maas-swagger.yml
  format: yaml
  label: Qubership MaaS (Messaging as a Service) API
  slug: qubership-maas-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/netcracker/refs/heads/main/openapi/netcracker-qubership-maas-swagger.yml
- filename: netcracker-qubership-dbaas-openapi.json
  format: json
  label: Qubership DBaaS Aggregator API
  slug: qubership-dbaas-aggregator-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/netcracker/refs/heads/main/openapi/netcracker-qubership-dbaas-openapi.json
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "sectigo.com"
  - 0 issue "symantec.com"
  - 0 iodef "mailto:postmaster@netcracker.com"
  - 0 issue "amazon.com"
  - 0 issue "digicert.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: netcracker.com
  spf: true
hosts:
- cert_expires: Aug  7 23:59:59 2026 GMT
  host: www.netcracker.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Netcracker Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Netcracker, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Netcracker
provider_slug: netcracker
slug: netcracker-domain-security
source_filename: netcracker-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-25'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.netcracker.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Aug  7 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: netcracker.com\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"symantec.com\"\n  - 0 iodef \"mailto:postmaster@netcracker.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"digicert.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/netcracker/refs/heads/main/security/netcracker-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Telecommunications
- United States
- BSS
- OSS
- Network Vendor
- API Management
- TM Forum
- OpenAPI
- CAMARA
- Standards
- Orchestration
- Monetization
- Open-Source
---
