---
api_specs:
- filename: polly-io-openapi-generated.yml
  format: yaml
  label: Polly API
  slug: polly-io-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/polly-io/refs/heads/main/openapi/_ae-authored/polly-io-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: polly.io
  spf: true
hosts:
- cert_expires: Jan  3 20:04:16 2027 GMT
  host: polly.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Polly Io Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Polly, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Polly
provider_slug: polly-io
slug: polly-io-domain-security
source_filename: polly-io-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-14'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: polly.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  3 20:04:16 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: polly.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/polly-io/refs/heads/main/security/polly-io-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- FinTech
- CapitalMarkets
- Mortgage
- APIPlatform
- AI
---
