---
api_specs:
- filename: openapi.yaml
  format: yaml
  label: Power Apps API
  slug: power-apps-api
  spec_type: OpenAPI
  url: https://docs.microsoft.com/en-us/connectors/powerappsforappmakers/
- filename: openapi
  format: yaml
  label: Dataverse API (Common Data Service)
  slug: dataverse-api-common-data-service
  spec_type: OpenAPI
  url: https://docs.microsoft.com/en-us/power-apps/developer/data-platform/webapi/openapi
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
- cert_expires: Dec 10 06:59:10 2026 GMT
  host: docs.microsoft.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan  5 22:51:40 2027 GMT
  host: api.powerapps.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan  4 01:54:17 2027 GMT
  host: api.bap.microsoft.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Microsoft Power Apps Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Microsoft Power Apps, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Microsoft Power Apps
provider_slug: microsoft-power-apps
slug: microsoft-power-apps-domain-security
source_filename: microsoft-power-apps-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: docs.microsoft.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 10 06:59:10 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.powerapps.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  5 22:51:40 2027 GMT\n  hsts: null\n- host: api.bap.microsoft.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  4 01:54:17 2027 GMT\n  hsts: null\ndomains:\n- domain: microsoft.com\n  dnssec: false\n  caa:\n  - 0 contactemail \"caarecordaware@microsoft.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: powerapps.com\n  dnssec: false\n  caa:\n  - 0 contactemail \"caarecordaware@microsoft.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/microsoft-power-apps/refs/heads/main/security/microsoft-power-apps-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Business Applications
- Cloud
- Enterprise
- Low-Code
- Microsoft
- No-Code
- Power Platform
- SaaS
---
