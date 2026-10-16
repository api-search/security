---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: puls.com
  spf: true
hosts:
- cert_expires: Mar 10 23:59:59 2027 GMT
  host: puls.com
  hsts: true
  hsts_max_age: 86400
  https: true
  tls_version: TLSv1.2
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Cellsavers Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cellsavers, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Cellsavers
provider_slug: cellsavers
slug: cellsavers-domain-security
source_filename: cellsavers-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-07'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: puls.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Mar 10 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 86400\ndomains:\n- domain: puls.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cellsavers/refs/heads/main/security/cellsavers-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Company
- HomeCare
- Repair
- Handyman
- SmartHome
- Services
---
