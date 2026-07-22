---
description: ''
domains:
- caa:
  - 0 issue "digicert.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: synthesized.io
  spf: true
hosts:
- cert_expires: Oct  7 12:02:59 2026 GMT
  host: synthesized.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Synthesized Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Synthesized, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Synthesized
provider_slug: synthesized
slug: synthesized-domain-security
source_filename: synthesized-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: synthesized.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  7 12:02:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: synthesized.io\n  dnssec: false\n  caa:\n  - 0 issue \"digicert.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/synthesized/refs/heads/main/security/synthesized-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Test Data
- Synthetic Data
- Data Masking
- Data Privacy
- Test Data Management
- Compliance
- Machine Learning
- Databases
- Developer Tools
---
