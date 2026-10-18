---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: mertech.com
  spf: true
hosts:
- cert_expires: Dec  8 01:01:52 2026 GMT
  host: mertech.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Mertech Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Mertech Data Systems, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Mertech Data Systems
provider_slug: mertech
slug: mertech-domain-security
source_filename: mertech-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: mertech.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  8 01:01:52 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: mertech.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mertech/refs/heads/main/security/mertech-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Application Modernization
- Database Migration
- Reporting Tools
- Web Services
- DataFlex
- Btrieve
---
