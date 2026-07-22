---
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: minimus.io
  spf: true
hosts:
- cert_expires: Aug 27 21:48:23 2026 GMT
  host: minimus.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Minimus Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Minimus, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Minimus
provider_slug: minimus
slug: minimus-domain-security
source_filename: minimus-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: minimus.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 27 21:48:23 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: minimus.io\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/minimus/refs/heads/main/security/minimus-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Container Images
- Container Security
- Supply Chain Security
- DevSecOps
- Compliance
- CLI
- Hardened Images
---
