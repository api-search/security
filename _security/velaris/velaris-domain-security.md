---
api_specs:
- filename: velaris-openapi.yml
  format: yaml
  label: Velaris Public API
  slug: velaris-public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/velaris/refs/heads/main/openapi/velaris-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: velaris.io
  spf: true
hosts:
- cert_expires: Dec 26 23:59:59 2026 GMT
  host: api.euw1.velaris.io
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Velaris Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Velaris, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Velaris
provider_slug: velaris
slug: velaris-domain-security
source_filename: velaris-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: api.euw1.velaris.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 26 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: velaris.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/velaris/refs/heads/main/security/velaris-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Customer Success
- AI
- SaaS
- Customer Data
- CRM
- Analytics
- Automation
- Company
---
