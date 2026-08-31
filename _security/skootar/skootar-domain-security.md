---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: skootar.com
  spf: true
hosts:
- cert_expires: Oct  6 09:28:29 2026 GMT
  host: skootar.com
  hsts: true
  hsts_max_age: 15724800
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Skootar Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Skootar, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Skootar
provider_slug: skootar
slug: skootar-domain-security
source_filename: skootar-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: skootar.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  6 09:28:29 2026 GMT\n  hsts: true\n  hsts_max_age: 15724800\ndomains:\n- domain: skootar.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/skootar/refs/heads/main/security/skootar-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Logistics
- Delivery
- Courier
- Messenger
- Last Mile
- Transportation
- Thailand
---
