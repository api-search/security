---
api_specs:
- filename: stepzen-admin-openapi.yml
  format: yaml
  label: StepZen Admin API
  slug: stepzen-admin-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stepzen/refs/heads/main/openapi/stepzen-admin-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "pki.goog"
  - 0 issue "amazonaws.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: stepzen.com
  spf: true
hosts:
- host: stepzen.com
  https: false
- cert_expires: Jan 10 23:59:59 2027 GMT
  host: dashboard.ibm.stepzen.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Stepzen Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for StepZen, probed live across 2 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: StepZen
provider_slug: stepzen
slug: stepzen-domain-security
source_filename: stepzen-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: stepzen.com\n  https: false\n- host: dashboard.ibm.stepzen.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 10 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: stepzen.com\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/stepzen/refs/heads/main/security/stepzen-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Backend Integration
- GraphQL
- API Gateway
- REST to GraphQL
- IBM
- Data Federation
---
