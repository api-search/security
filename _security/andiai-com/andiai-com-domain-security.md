---
api_specs:
- filename: andiai-com-search-api-openapi.yml
  format: yaml
  label: Andi AI Search API
  slug: andiai-com-search-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/andiai-com/openapi/andiai-com-search-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: andiai.com
  spf: true
hosts:
- cert_expires: Jan 12 17:12:04 2027 GMT
  host: andiai.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Andi AI Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Andi AI, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Andi AI
provider_slug: andiai-com
slug: andiai-com-domain-security
source_filename: andiai-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-01'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: andiai.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 12 17:12:04 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: andiai.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/andiai-com/security/andiai-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Artificial Intelligence
- Search
- Privacy
- OpenAI
- Community
---
