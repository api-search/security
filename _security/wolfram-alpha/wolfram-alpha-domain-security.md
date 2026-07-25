---
api_specs:
- filename: wolfram-alpha-queries-api-openapi.yml
  format: yaml
  label: Wolfram|Alpha Queries API
  slug: wolfram-alpha-queries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wolfram-alpha/refs/heads/main/openapi/wolfram-alpha-queries-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: wolframalpha.com
  spf: true
hosts:
- cert_expires: Dec  3 16:16:35 2026 GMT
  host: www.wolframalpha.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec  3 16:16:35 2026 GMT
  host: products.wolframalpha.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec  3 16:16:35 2026 GMT
  host: api.wolframalpha.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Wolfram Alpha Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Wolfram|Alpha, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Wolfram|Alpha
provider_slug: wolfram-alpha
slug: wolfram-alpha-domain-security
source_filename: wolfram-alpha-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.wolframalpha.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  3 16:16:35 2026 GMT\n  hsts: null\n- host: products.wolframalpha.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  3 16:16:35 2026 GMT\n  hsts: null\n- host: api.wolframalpha.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  3 16:16:35 2026 GMT\n  hsts: null\ndomains:\n- domain: wolframalpha.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wolfram-alpha/refs/heads/main/security/wolfram-alpha-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- AI
- Artificial Intelligence
- Computational Knowledge
- Natural Language Processing
- Search
---
