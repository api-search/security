---
api_specs:
- filename: crescendo-lab-maacgo-openapi.yaml
  format: yaml
  label: MAAC Go API
  slug: maac-go-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/crescendo-lab/refs/heads/main/openapi/crescendo-lab-maacgo-openapi.yaml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: cresclab.com
  spf: true
hosts:
- cert_expires: Sep 17 08:31:28 2026 GMT
  host: cresclab.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Crescendo Lab Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Crescendo Lab, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Crescendo Lab
provider_slug: crescendo-lab
slug: crescendo-lab-domain-security
source_filename: crescendo-lab-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: cresclab.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 17 08:31:28 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: cresclab.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/crescendo-lab/refs/heads/main/security/crescendo-lab-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- SMS
- Messaging
- Marketing Automation
- Customer Engagement
- Taiwan
- Omnichannel
- MCP
---
