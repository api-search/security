---
api_specs:
- filename: microsoft-power-automate-management-api.yaml
  format: yaml
  label: Power Automate Management API
  slug: power-automate-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-power-automate/refs/heads/main/openapi/microsoft-power-automate-management-api.yaml
description: ''
domains:
- caa:
  - 0 contactemail "caarecordaware@microsoft.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: powerautomate.com
  spf: false
- caa:
  - 0 contactemail "caarecordaware@microsoft.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: microsoft.com
  spf: true
hosts:
- cert_expires: Jan  5 22:51:39 2027 GMT
  host: make.powerautomate.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 11 02:26:09 2026 GMT
  host: learn.microsoft.com
  hsts: true
  hsts_max_age: 31536000
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
name: Microsoft Power Automate Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Microsoft Power Automate, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=reject).'
provider_name: Microsoft Power Automate
provider_slug: microsoft-power-automate
slug: microsoft-power-automate-domain-security
source_filename: microsoft-power-automate-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: make.powerautomate.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  5 22:51:39 2027 GMT\n  hsts: null\n- host: learn.microsoft.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 11 02:26:09 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.flow.microsoft.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  4 01:52:17 2027 GMT\n  hsts: null\ndomains:\n- domain: powerautomate.com\n  dnssec: false\n  caa:\n  - 0 contactemail \"caarecordaware@microsoft.com\"\n  spf: false\n  dmarc: true\n  dmarc_policy: reject\n- domain: microsoft.com\n  dnssec: false\n  caa:\n  - 0 contactemail \"caarecordaware@microsoft.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/microsoft-power-automate/refs/heads/main/security/microsoft-power-automate-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Automation
- Business Process
- Integration
- Low-Code
- Microsoft
- Power Platform
- RPA
- Workflow
---
