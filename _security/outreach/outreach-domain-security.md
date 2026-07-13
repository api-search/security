---
api_specs:
- filename: outreach-webhooks-asyncapi.yml
  format: yaml
  label: Outreach Webhooks
  slug: outreach-webhooks
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/outreach/refs/heads/main/webhooks/outreach-webhooks-asyncapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: outreach.io
  spf: true
hosts:
- cert_expires: Dec 23 23:59:59 2026 GMT
  host: www.outreach.io
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 13 23:59:59 2026 GMT
  host: developers.outreach.io
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 13 23:59:59 2027 GMT
  host: api.outreach.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Outreach Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Outreach, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Outreach
provider_slug: outreach
slug: outreach-domain-security
source_filename: outreach-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.outreach.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 23 23:59:59 2026 GMT\n  hsts: false\n- host: developers.outreach.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 13 23:59:59 2026 GMT\n  hsts: false\n- host: api.outreach.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 13 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: outreach.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/outreach/refs/heads/main/security/outreach-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Sales
- Sales Engagement
- Sequences
- CRM
- Email
---
