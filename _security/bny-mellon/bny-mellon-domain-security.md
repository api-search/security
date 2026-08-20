---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: bny.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: bnymellon.com
  spf: true
hosts:
- cert_expires: Feb  2 23:59:59 2027 GMT
  host: www.bny.com
  hsts: true
  hsts_max_age: 86400
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 14 23:59:59 2027 GMT
  host: marketplace.bnymellon.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
- cert_expires: Dec 20 23:59:59 2026 GMT
  host: developer.bny.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Bny Mellon Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for BNY Mellon, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: BNY Mellon
provider_slug: bny-mellon
slug: bny-mellon-domain-security
source_filename: bny-mellon-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-23'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.bny.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  2 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 86400\n- host: marketplace.bnymellon.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jan 14 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developer.bny.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 20 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: bny.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: bnymellon.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bny-mellon/refs/heads/main/security/bny-mellon-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Financial-Services
- Banking
- United States
- Custody Bank
- Treasury Services
- Payments
- Digital Assets
- Open Finance
---
