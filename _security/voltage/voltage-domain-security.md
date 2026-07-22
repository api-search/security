---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: voltage.cloud
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: voltageapi.com
  spf: false
hosts:
- cert_expires: Oct 10 10:03:46 2026 GMT
  host: voltage.cloud
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 27 02:49:11 2026 GMT
  host: docs.voltageapi.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug  3 13:07:08 2026 GMT
  host: voltageapi.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Voltage Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Voltage, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Voltage
provider_slug: voltage
slug: voltage-domain-security
source_filename: voltage-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: voltage.cloud\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 10 10:03:46 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.voltageapi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 27 02:49:11 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: voltageapi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug  3 13:07:08 2026 GMT\n  hsts: null\ndomains:\n- domain: voltage.cloud\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: voltageapi.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/voltage/refs/heads/main/security/voltage-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Enterprise
- Bitcoin
- Lightning Network
- Payments
- Cryptocurrency
- Financial Services
- Wallets
- Infrastructure
- Fintech
- Node Hosting
- Web3
---
