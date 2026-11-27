---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: true
  domain: gtinfetch.ai
  spf: false
hosts:
- cert_expires: Jan 10 04:11:26 2027 GMT
  host: gtinfetch.ai
  hsts: true
  hsts_max_age: 10886400
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: GTINFetch AI Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for GTINFetch AI, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF absent, DMARC absent.'
provider_name: GTINFetch AI
provider_slug: gtinfetch-ai
slug: gtinfetch-ai-domain-security
source_filename: gtinfetch-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-10'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: gtinfetch.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 10 04:11:26 2027 GMT\n  hsts: true\n  hsts_max_age: 10886400\ndomains:\n- domain: gtinfetch.ai\n  dnssec: true\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/gtinfetch-ai/security/gtinfetch-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC
tags:
- GTIN
- Barcode Lookup
- AI Agents
- Retail Grocery
---
