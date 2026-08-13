---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: arqfinance.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: dolarapp.com
  spf: true
hosts:
- cert_expires: Jan  8 23:59:59 2027 GMT
  host: www.arqfinance.com
  hsts: true
  hsts_max_age: 86400000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 31 05:23:01 2026 GMT
  host: status.dolarapp.com
  hsts: true
  hsts_max_age: 259200
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Dolarapp Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for DolarApp, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: DolarApp
provider_slug: dolarapp
slug: dolarapp-domain-security
source_filename: dolarapp-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.arqfinance.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  8 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 86400000\n- host: status.dolarapp.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 31 05:23:01 2026 GMT\n  hsts: true\n  hsts_max_age: 259200\ndomains:\n- domain: arqfinance.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: dolarapp.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dolarapp/refs/heads/main/security/dolarapp-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Fintech
- Payments
- Cross-Border Payments
- Banking
- Digital Dollars
- Stablecoins
- Foreign Exchange
- Corporate Cards
- Latin America
---
