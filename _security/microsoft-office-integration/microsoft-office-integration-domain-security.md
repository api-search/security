---
api_specs:
- filename: microsoft-office-management-activity-api-openapi.yml
  format: yaml
  label: Microsoft Office 365 Management Activity API
  slug: management-activity-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-office-integration/refs/heads/main/openapi/microsoft-office-management-activity-api-openapi.yml
- filename: microsoft-office-service-communications-api-openapi.yml
  format: yaml
  label: Microsoft Office 365 Service Communications API
  slug: service-communications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-office-integration/refs/heads/main/openapi/microsoft-office-service-communications-api-openapi.yml
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
- cert_expires: Nov 20 02:11:36 2026 GMT
  host: developer.microsoft.com
  hsts: true
  hsts_max_age: 31536000
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
name: Microsoft Office Integration Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Microsoft Office Integration, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Microsoft Office Integration
provider_slug: microsoft-office-integration
slug: microsoft-office-integration-domain-security
source_filename: microsoft-office-integration-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developer.microsoft.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 20 02:11:36 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: learn.microsoft.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 11 02:26:09 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: microsoft.com\n  dnssec: false\n  caa:\n  - 0 contactemail \"caarecordaware@microsoft.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/microsoft-office-integration/refs/heads/main/security/microsoft-office-integration-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Microsoft 365
- Microsoft Office Integration
- Office 365
---
