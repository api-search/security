---
api_specs:
- filename: vbout-openapi-original.json
  format: json
  label: VBOUT API
  slug: vbout-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vbout/refs/heads/main/openapi/vbout-openapi-original.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: vbout.com
  spf: true
hosts:
- cert_expires: Oct  5 15:35:38 2026 GMT
  host: vbout.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  5 15:35:38 2026 GMT
  host: api.vbout.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Vbout Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for VBOUT, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: VBOUT
provider_slug: vbout
slug: vbout-domain-security
source_filename: vbout-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: vbout.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  5 15:35:38 2026 GMT\n  hsts: false\n- host: api.vbout.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  5 15:35:38 2026 GMT\n  hsts: false\ndomains:\n- domain: vbout.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vbout/refs/heads/main/security/vbout-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Marketing Automation
- Email Marketing
- Social Media
- Lead Management
- Landing Pages
- Chatbots
- Contacts
- Campaigns
- SaaS
---
