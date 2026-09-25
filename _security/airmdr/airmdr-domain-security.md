---
api_specs:
- filename: airmdr-case-manager-openapi.yml
  format: yaml
  label: AirMDR Case Manager API
  slug: airmdr-case-manager-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/airmdr/refs/heads/main/openapi/airmdr-case-manager-openapi.yml
- filename: airmdr-user-management-service-openapi.yml
  format: yaml
  label: AirMDR User Management Service API
  slug: airmdr-user-management-service-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/airmdr/refs/heads/main/openapi/airmdr-user-management-service-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: airmdr.com
  spf: true
hosts:
- cert_expires: Nov 28 14:01:11 2026 GMT
  host: airmdr.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 25 23:59:59 2026 GMT
  host: app.airmdr.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 26 23:17:05 2026 GMT
  host: docs.airmdr.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Airmdr Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AirMDR, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: AirMDR
provider_slug: airmdr
slug: airmdr-domain-security
source_filename: airmdr-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: airmdr.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 28 14:01:11 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: app.airmdr.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 25 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.airmdr.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 26 23:17:05 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: airmdr.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/airmdr/refs/heads/main/security/airmdr-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Security
- Managed Detection and Response
- Security Operations
- Alert Triage
- Incident Response
- AI Agents
- SOC Automation
- Threat Detection
- MCP
- A2A
---
