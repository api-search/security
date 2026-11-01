---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: ecobites.net
  spf: true
hosts:
- cert_expires: Jan 18 22:25:05 2027 GMT
  host: www.ecobites.net
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Rec Rec Vn Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Ecobites Pte. Ltd., probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Ecobites Pte. Ltd.
provider_slug: rec-rec-vn
slug: rec-rec-vn-domain-security
source_filename: rec-rec-vn-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-25'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.ecobites.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 18 22:25:05 2027 GMT\n  hsts: false\ndomains:\n- domain: ecobites.net\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/rec-rec-vn/security/rec-rec-vn-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- FoodTech
- API
- Singapore
- Marketplace
---
