---
description: ''
domains:
- caa:
  - 0 issue "amazon.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 issuewild ";"
  - 0 iodef "mailto:infosec@hummingbird.co"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: hummingbird.co
  spf: true
hosts:
- cert_expires: Aug 22 13:35:31 2026 GMT
  host: hummingbird.co
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Hummingbird Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Hummingbird, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Hummingbird
provider_slug: hummingbird
slug: hummingbird-domain-security
source_filename: hummingbird-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: hummingbird.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 22 13:35:31 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: hummingbird.co\n  dnssec: false\n  caa:\n  - 0 issue \"amazon.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 issuewild \";\"\n  - 0 iodef \"mailto:infosec@hummingbird.co\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hummingbird/refs/heads/main/security/hummingbird-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Fintech
- Compliance
- RegTech
- Anti-Money-Laundering
- Financial Crime
- Transaction Monitoring
- Regulatory Reporting
---
