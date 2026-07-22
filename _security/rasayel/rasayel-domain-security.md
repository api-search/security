---
api_specs:
- filename: rasayel-rest-openapi.yml
  format: yaml
  label: Rasayel REST API
  slug: rasayel-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rasayel/refs/heads/main/openapi/rasayel-rest-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: rasayel.io
  spf: true
hosts:
- cert_expires: Sep  4 15:39:49 2026 GMT
  host: rasayel.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Rasayel Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Rasayel, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Rasayel
provider_slug: rasayel
slug: rasayel-domain-security
source_filename: rasayel-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: rasayel.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  4 15:39:49 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: rasayel.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rasayel/refs/heads/main/security/rasayel-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- WhatsApp
- Messaging
- Business Messaging
- Sales
- CRM
- Customer Communication
- Conversational Commerce
- API
---
