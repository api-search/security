---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: emidat.com
  spf: true
hosts:
- cert_expires: Oct 15 23:18:11 2026 GMT
  host: www.emidat.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Emidat Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Emidat, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Emidat
provider_slug: emidat
slug: emidat-domain-security
source_filename: emidat-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.emidat.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 15 23:18:11 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: emidat.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/emidat/refs/heads/main/security/emidat-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Construction
- Sustainability
- Environmental Product Declaration
- EPD
- Life Cycle Assessment
- Digital Product Passport
- Carbon
- Climate
- Building Materials
---
