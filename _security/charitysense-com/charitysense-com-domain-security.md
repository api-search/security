---
api_specs:
- filename: charitysense-com-openapi.yml
  format: yaml
  label: CharitySense Data API
  slug: charitysense-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/charitysense-com/refs/heads/main/openapi/charitysense-com-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: charitysense.com
  spf: false
hosts:
- cert_expires: Nov  8 16:01:36 2026 GMT
  host: charitysense.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  8 16:01:36 2026 GMT
  host: data.charitysense.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 2
kind: domain-security
layout: security
method: probed
name: Charitysense Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for CharitySense, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: CharitySense
provider_slug: charitysense-com
slug: charitysense-com-domain-security
source_filename: charitysense-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: charitysense.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  8 16:01:36 2026 GMT\n  hsts: false\n- host: data.charitysense.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  8 16:01:36 2026 GMT\n  hsts: false\ndomains:\n- domain: charitysense.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/charitysense-com/refs/heads/main/security/charitysense-com-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Non-Profit
- Charities
- Due Diligence
- IRS Form 990
- Donor Research
- Grants
- Philanthropy
- Open Data
- Agents
- A2A
- Impact Verification
- Edge AI
- United States
- Company
---
