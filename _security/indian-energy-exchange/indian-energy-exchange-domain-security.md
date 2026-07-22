---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: iexindia.com
  spf: true
hosts:
- cert_expires: Jul 29 23:59:59 2026 GMT
  host: www.iexindia.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Indian Energy Exchange Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Indian Energy Exchange, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Indian Energy Exchange
provider_slug: indian-energy-exchange
slug: indian-energy-exchange-domain-security
source_filename: indian-energy-exchange-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.iexindia.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jul 29 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: iexindia.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/indian-energy-exchange/refs/heads/main/security/indian-energy-exchange-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Energy
- Electricity
- Power Trading
- Exchange
- Marketplace
- Renewable Energy
- Trading
- India
---
