---
description: ''
domains:
- caa:
  - 0 issue "pki.goog"
  - 0 issue "amazon.com"
  - 0 issue "digicert.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: zylo.com
  spf: true
hosts:
- cert_expires: Oct  1 02:30:41 2026 GMT
  host: zylo.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  7 21:26:49 2026 GMT
  host: developer.zylo.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Cleanshelf Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cleanshelf, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Cleanshelf
provider_slug: cleanshelf
slug: cleanshelf-domain-security
source_filename: cleanshelf-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: zylo.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 02:30:41 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developer.zylo.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  7 21:26:49 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: zylo.com\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cleanshelf/refs/heads/main/security/cleanshelf-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Acquired
- License Management
- SaaS Management
- Shadow IT
- SMP
- Software Asset Management
- Spend Optimization
---
