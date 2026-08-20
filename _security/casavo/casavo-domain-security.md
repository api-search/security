---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: casavo.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: realisti.co
  spf: true
hosts:
- cert_expires: Oct 15 22:37:59 2026 GMT
  host: casavo.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec  9 23:59:59 2026 GMT
  host: editor.realisti.co
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Casavo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Casavo, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Casavo
provider_slug: casavo
slug: casavo-domain-security
source_filename: casavo-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-09'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: casavo.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 15 22:37:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: editor.realisti.co\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec  9 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: casavo.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: realisti.co\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/casavo/refs/heads/main/security/casavo-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Real-Estate
- PropTech
- Marketplace
- Virtual Tours
- Property Listings
- Italy
- Spain
- France
- Mortgages
---
