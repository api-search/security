---
api_specs:
- filename: openapi
  format: yaml
  label: Blend API
  slug: blend-api
  spec_type: OpenAPI
  url: https://developers.blend.com/blend/openapi
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: blend.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: blendlabs.com
  spf: true
hosts:
- cert_expires: Aug 14 03:22:33 2026 GMT
  host: blend.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.2
- cert_expires: Oct  4 02:53:41 2026 GMT
  host: developers.blend.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 18 23:59:59 2026 GMT
  host: api.blendlabs.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Blend Labs Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Blend Labs, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.2); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Blend Labs
provider_slug: blend-labs
slug: blend-labs-domain-security
source_filename: blend-labs-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: blend.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Aug 14 03:22:33 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: developers.blend.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 02:53:41 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.blendlabs.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 18 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: blend.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: blendlabs.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/blend-labs/refs/heads/main/security/blend-labs-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Company
- Financial Services
- Mortgage
- Lending
- Banking
- Digital Banking
- Fintech
- Account Opening
- Mortgage Technology
- Consumer Lending
- Deposit Accounts
- Verification
- eClosing
---
