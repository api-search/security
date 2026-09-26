---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: arival.com
  spf: true
hosts:
- cert_expires: Nov 12 07:29:50 2026 GMT
  host: arival.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Arivalbank Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Arivalbank, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Arivalbank
provider_slug: arivalbank
slug: arivalbank-domain-security
source_filename: arivalbank-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: arival.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 12 07:29:50 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: arival.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/arivalbank/refs/heads/main/security/arivalbank-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- FinTech
- Banking
- DigitalBanking
- GlobalPayments
- Stablecoins
---
