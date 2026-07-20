---
description: ''
domains:
- caa:
  - 0 issue "pki.goog"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: celona.io
  spf: true
hosts:
- cert_expires: Oct 14 05:12:24 2026 GMT
  host: celona.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Celona Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Celona, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Celona
provider_slug: celona
slug: celona-domain-security
source_filename: celona-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: celona.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 14 05:12:24 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: celona.io\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/celona/refs/heads/main/security/celona-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Networking
- Private Cellular
- 5G
- LTE
- CBRS
- Wireless
- Network Monitoring
- Telecommunications
- IoT
---
