---
description: ''
domains:
- caa:
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "godaddy.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "ssl.com"
  - 0 issuewild "comodoca.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: bensonhill.com
  spf: true
hosts:
- cert_expires: Sep 28 10:55:00 2026 GMT
  host: bensonhill.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Benson Hill Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Benson Hill *, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Benson Hill *
provider_slug: benson-hill
slug: benson-hill-domain-security
source_filename: benson-hill-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: bensonhill.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 28 10:55:00 2026 GMT\n  hsts: false\ndomains:\n- domain: bensonhill.com\n  dnssec: false\n  caa:\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"godaddy.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"comodoca.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/benson-hill/refs/heads/main/security/benson-hill-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Frontier Tech
- Agriculture
- AgTech
- Food Tech
- Biotechnology
- Crop Genetics
- Soybean
---
