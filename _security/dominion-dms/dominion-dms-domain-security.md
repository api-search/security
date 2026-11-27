---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: dominiondms.com
  spf: true
hosts:
- cert_expires: Dec 10 02:12:45 2026 GMT
  host: dominiondms.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Dominion DMS Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Dominion DMS, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Dominion DMS
provider_slug: dominion-dms
slug: dominion-dms-domain-security
source_filename: dominion-dms-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-16'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: dominiondms.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 10 02:12:45 2026 GMT\n  hsts: false\ndomains:\n- domain: dominiondms.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/dominion-dms/security/dominion-dms-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Dealer Management
- Software
- Automotive
- CRM
- Cloud
---
