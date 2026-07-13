---
api_specs:
- filename: openapi.yaml
  format: yaml
  label: Power Apps REST API
  slug: power-apps-rest-api
  spec_type: OpenAPI
  url: https://learn.microsoft.com/en-us/connectors/powerappsforappmakers/
- filename: openapi
  format: yaml
  label: Microsoft Dataverse Web API
  slug: microsoft-dataverse-web-api
  spec_type: OpenAPI
  url: https://learn.microsoft.com/en-us/power-apps/developer/data-platform/webapi/openapi
description: ''
domains:
- caa:
  - 0 contactemail "caarecordaware@microsoft.com"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: powerapps.com
  spf: true
- caa:
  - 0 contactemail "caarecordaware@microsoft.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: microsoft.com
  spf: true
hosts:
- cert_expires: Jan  5 22:51:38 2027 GMT
  host: make.powerapps.com
  hsts: null
  https: true
  tls_version: TLSv1.3
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
kind: domain-security
layout: security
method: probed
name: Power Apps Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Microsoft Power Apps, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Microsoft Power Apps
provider_slug: power-apps
slug: power-apps-domain-security
source_filename: power-apps-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: make.powerapps.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  5 22:51:38 2027 GMT\n  hsts: null\n- host: docs.microsoft.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 10 06:59:10 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.powerapps.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  5 22:51:40 2027 GMT\n  hsts: null\ndomains:\n- domain: powerapps.com\n  dnssec: false\n  caa:\n  - 0 contactemail \"caarecordaware@microsoft.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: microsoft.com\n  dnssec: false\n  caa:\n  - 0 contactemail \"caarecordaware@microsoft.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/power-apps/refs/heads/main/security/power-apps-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- App Development
- Business Applications
- Cloud Platform
- Low-Code
- Microsoft
- No-Code
---
