---
api_specs:
- filename: v1
  format: yaml
  label: Power Apps API
  slug: power-apps-api
  spec_type: OpenAPI
  url: https://api.powerapps.com/openapi/v1
- filename: v1
  format: yaml
  label: Power Automate API
  slug: power-automate-api
  spec_type: OpenAPI
  url: https://api.flow.microsoft.com/openapi/v1
- filename: swagger.json
  format: json
  label: Power BI REST API
  slug: power-bi-rest-api
  spec_type: OpenAPI
  url: https://api.powerbi.com/v1.0/myorg/swagger.json
- filename: power-platform-api-openapi.json
  format: json
  label: Power Platform Unified API
  slug: power-platform-unified-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/power-platform/refs/heads/main/openapi/power-platform-api-openapi.json
description: ''
domains:
- caa:
  - 0 contactemail "caarecordaware@microsoft.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: microsoft.com
  spf: true
- caa:
  - 0 contactemail "caarecordaware@microsoft.com"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: powerapps.com
  spf: true
hosts:
- cert_expires: Dec 11 02:26:09 2026 GMT
  host: learn.microsoft.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan  5 22:51:40 2027 GMT
  host: api.powerapps.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan  4 01:52:17 2027 GMT
  host: api.flow.microsoft.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Power Platform Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Microsoft Power Platform APIs, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Microsoft Power Platform APIs
provider_slug: power-platform
slug: power-platform-domain-security
source_filename: power-platform-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: learn.microsoft.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 11 02:26:09 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.powerapps.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  5 22:51:40 2027 GMT\n  hsts: null\n- host: api.flow.microsoft.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  4 01:52:17 2027 GMT\n  hsts: null\ndomains:\n- domain: microsoft.com\n  dnssec: false\n  caa:\n  - 0 contactemail \"caarecordaware@microsoft.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: powerapps.com\n  dnssec: false\n  caa:\n  - 0 contactemail \"caarecordaware@microsoft.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/power-platform/refs/heads/main/security/power-platform-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Business Applications
- Copilot Studio
- Dataverse
- Low-Code
- Microsoft
- No-Code
- Power Pages
- Power Platform
---
