---
api_specs:
- filename: try_api_online
  format: yaml
  label: Sardine API
  slug: sardine-api
  spec_type: OpenAPI
  url: https://docs.sardine.ai/try_api_online
description: ''
domains:
- caa:
  - 0 issuewild "pki.goog"
  - 0 issue "amazonaws.com"
  - 0 issuewild "letsencrypt.org"
  - 0 issue "letsencrypt.org"
  - 0 issue "globalsign.com"
  - 0 issue "pki.goog"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: sardine.ai
  spf: true
hosts:
- cert_expires: Sep 18 22:26:11 2026 GMT
  host: www.sardine.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 26 07:59:40 2026 GMT
  host: docs.sardine.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 29 20:08:04 2026 GMT
  host: api.sardine.ai
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Sardine Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Sardine, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Sardine
provider_slug: sardine
slug: sardine-domain-security
source_filename: sardine-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.sardine.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 18 22:26:11 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.sardine.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 26 07:59:40 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.sardine.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 20:08:04 2026 GMT\n  hsts: null\ndomains:\n- domain: sardine.ai\n  dnssec: false\n  caa:\n  - 0 issuewild \"pki.goog\"\n  - 0 issue \"amazonaws.com\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"globalsign.com\"\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sardine/refs/heads/main/security/sardine-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Fraud Prevention
- AML
- Compliance
- KYC
- KYB
- Device Intelligence
- Behavior Biometrics
- Transaction Risk
- Financial Crime
- Identity Verification
- Chargeback Protection
- FinTech
---
