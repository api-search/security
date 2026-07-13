---
api_specs:
- filename: kagi-openapi.yml
  format: yaml
  label: Kagi Search API
  slug: search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kagi/refs/heads/main/openapi/kagi-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: kagi.com
  spf: true
hosts:
- cert_expires: Sep 25 13:45:46 2026 GMT
  host: kagi.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 25 13:45:46 2026 GMT
  host: help.kagi.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Kagi Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Kagi, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Kagi
provider_slug: kagi
slug: kagi-domain-security
source_filename: kagi-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: kagi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 25 13:45:46 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: help.kagi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 25 13:45:46 2026 GMT\n  hsts: false\ndomains:\n- domain: kagi.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kagi/refs/heads/main/security/kagi-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Search
- Premium Search
- AI Search
- Summarization
- FastGPT
- Enrichment
- OpenAPI
- Pay-Per-Use
- Privacy
- LLMs
- Web Index
---
