---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: bridgewaterbank.ca
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: bwbbrokerinfo.ca
  spf: false
hosts:
- cert_expires: Nov  6 14:23:01 2026 GMT
  host: www.bridgewaterbank.ca
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 20 20:53:04 2026 GMT
  host: bwbbrokerinfo.ca
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Bridgewater Bank Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Bridgewater Bank, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Bridgewater Bank
provider_slug: bridgewater-bank
slug: bridgewater-bank-domain-security
source_filename: bridgewater-bank-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-23'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.bridgewaterbank.ca\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  6 14:23:01 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: bwbbrokerinfo.ca\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 20 20:53:04 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: bridgewaterbank.ca\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: bwbbrokerinfo.ca\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bridgewater-bank/refs/heads/main/security/bridgewater-bank-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Financial Services
- Banking
- Canada
- Schedule I Bank
- Mortgages
- Deposits
- Brokers
- Alberta
- Open Banking
---
