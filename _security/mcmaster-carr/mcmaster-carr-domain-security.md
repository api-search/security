---
description: ''
domains:
- caa:
  - 0 issue "digicert.com"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: mcmaster.com
  spf: true
hosts:
- cert_expires: May 14 23:59:59 2027 GMT
  host: mcmaster.com
  hsts: false
  https: true
  tls_version: TLSv1.2
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: McMaster-Carr Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for McMaster-Carr, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: McMaster-Carr
provider_slug: mcmaster-carr
slug: mcmaster-carr-domain-security
source_filename: mcmaster-carr-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-16'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: mcmaster.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: May 14 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: mcmaster.com\n  dnssec: false\n  caa:\n  - 0 issue \"digicert.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/mcmaster-carr/security/mcmaster-carr-domain-security.yml
summary_line: TLSv1.2 · DMARC
tags:
- Company
- Industrial
- Supplies
- Catalog
- Engineering
---
