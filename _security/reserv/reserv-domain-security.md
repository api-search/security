---
description: ''
domains:
- caa:
  - 0 issue "amazontrust.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "amazon.com"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: reserv.com
  spf: true
hosts:
- cert_expires: Sep 13 01:38:40 2026 GMT
  host: reserv.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Reserv Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Reserv, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Reserv
provider_slug: reserv
slug: reserv-domain-security
source_filename: reserv-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: reserv.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 13 01:38:40 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: reserv.com\n  dnssec: false\n  caa:\n  - 0 issue \"amazontrust.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"amazon.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/reserv/refs/heads/main/security/reserv-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Insurance
- Claims Management
- Insurtech
- Third-Party Administrator
- Property & Casualty
- Artificial Intelligence
- Data Analytics
---
