---
api_specs:
- filename: bounti-content-api-openapi.json
  format: json
  label: Bounti.ai Content API
  slug: bountiai-content-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bounti/refs/heads/main/openapi/bounti-content-api-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: bounti.ai
  spf: true
hosts:
- cert_expires: Sep 10 01:36:03 2026 GMT
  host: bounti.ai
  hsts: true
  hsts_max_age: 31556926
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Bounti Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Bounti, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Bounti
provider_slug: bounti
slug: bounti-domain-security
source_filename: bounti-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: bounti.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 10 01:36:03 2026 GMT\n  hsts: true\n  hsts_max_age: 31556926\ndomains:\n- domain: bounti.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bounti/refs/heads/main/security/bounti-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Real Estate
- Artificial Intelligence
- Marketing
- Sales Enablement
- Virtual Staging
- Content Generation
- AI Agents
---
