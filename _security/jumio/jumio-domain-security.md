---
api_specs:
- filename: jumio-callback-asyncapi.yml
  format: yaml
  label: Jumio Callback / Webhook
  slug: callback
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/jumio/refs/heads/main/asyncapi/jumio-callback-asyncapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: jumio.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: jumio.ai
  spf: false
hosts:
- cert_expires: Sep 14 15:59:48 2026 GMT
  host: www.jumio.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec  1 23:59:59 2026 GMT
  host: documentation.jumio.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 26 23:59:59 2026 GMT
  host: account.amer-1.jumio.ai
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Jumio Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Jumio, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Jumio
provider_slug: jumio
slug: jumio-domain-security
source_filename: jumio-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.jumio.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 15:59:48 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: documentation.jumio.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  1 23:59:59 2026 GMT\n  hsts: false\n- host: account.amer-1.jumio.ai\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep 26 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: jumio.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: jumio.ai\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/jumio/refs/heads/main/security/jumio-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- KYC
- Identity Verification
- Biometrics
- AML
- Fraud Prevention
- KYX
---
