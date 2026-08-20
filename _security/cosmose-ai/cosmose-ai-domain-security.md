---
api_specs:
- filename: cosmose-ai-deal-hunter-registration-api-openapi.yml
  format: yaml
  label: Cosmose AI Deal Hunter Registration API
  slug: cosmose-ai-deal-hunter-registration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cosmose-ai/refs/heads/main/openapi/cosmose-ai-deal-hunter-registration-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: cosmose.ai
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: cosmose.co
  spf: true
hosts:
- cert_expires: Dec  1 23:59:59 2026 GMT
  host: cosmose.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 13 02:35:59 2026 GMT
  host: api.sg.cosmose.co
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Cosmose Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cosmose AI, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Cosmose AI
provider_slug: cosmose-ai
slug: cosmose-ai-domain-security
source_filename: cosmose-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: cosmose.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  1 23:59:59 2026 GMT\n  hsts: false\n- host: api.sg.cosmose.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 13 02:35:59 2026 GMT\n  hsts: null\ndomains:\n- domain: cosmose.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n- domain: cosmose.co\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cosmose-ai/refs/heads/main/security/cosmose-ai-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Retail Intelligence
- offline-analytics
- Location Intelligence
- AdTech
- consumer-behavior
- Shopper Analytics
- Mobile SDK
- Advertising
- Artificial Intelligence
- Singapore
---
