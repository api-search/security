---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: exxpertapps.com
  spf: true
hosts:
- cert_expires: Feb 24 23:59:59 2027 GMT
  host: exxpertapps.com
  hsts: false
  https: true
  tls_version: TLSv1.2
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Exxpertapps Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Calvi Systems SL, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Calvi Systems SL
provider_slug: exxpertapps
slug: exxpertapps-domain-security
source_filename: exxpertapps-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: exxpertapps.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Feb 24 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: exxpertapps.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/exxpertapps/security/exxpertapps-domain-security.yml
summary_line: TLSv1.2 · DMARC
tags:
- CRM
- Project Management
- Billing
- B2B Services
- Multi-Currency
- ERP Integration
---
