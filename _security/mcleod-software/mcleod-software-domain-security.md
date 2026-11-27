---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: mcleodsoftware.com
  spf: true
hosts:
- cert_expires: Feb  2 05:49:33 2027 GMT
  host: mcleodsoftware.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: McLeod LoadMaster Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for McLeod LoadMaster, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: McLeod LoadMaster
provider_slug: mcleod-software
slug: mcleod-software-domain-security
source_filename: mcleod-software-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-15'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: mcleodsoftware.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  2 05:49:33 2027 GMT\n  hsts: null\ndomains:\n- domain: mcleodsoftware.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/mcleod-software/security/mcleod-software-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Transportation
- Logistics
- Software
- TMS
- Freight
---
