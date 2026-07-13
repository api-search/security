---
description: ''
domains:
- caa:
  - 0 issue "pki.goog"
  - 0 issue "letsencrypt.org"
  - 0 iodef "mailto:security@hyperproof.io"
  - 0 issue "digicert.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: hyperproof.io
  spf: true
hosts:
- cert_expires: Aug 18 21:21:30 2026 GMT
  host: hyperproof.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- host: developers.hyperproof.io
  https: false
kind: domain-security
layout: security
method: probed
name: Hyperproof Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Hyperproof, probed live across 2 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Hyperproof
provider_slug: hyperproof
slug: hyperproof-domain-security
source_filename: hyperproof-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: hyperproof.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 18 21:21:30 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developers.hyperproof.io\n  https: false\ndomains:\n- domain: hyperproof.io\n  dnssec: true\n  caa:\n  - 0 issue \"pki.goog\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 iodef \"mailto:security@hyperproof.io\"\n  - 0 issue \"digicert.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hyperproof/refs/heads/main/security/hyperproof-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- GRC
- Compliance
- Risk
- Audit
- SOC 2
---
