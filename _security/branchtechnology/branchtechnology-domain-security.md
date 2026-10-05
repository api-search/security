---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: branchtechnology.com
  spf: true
hosts:
- cert_expires: Dec 11 03:14:29 2026 GMT
  host: branchtechnology.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Branchtechnology Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Branchtechnology, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Branchtechnology
provider_slug: branchtechnology
slug: branchtechnology-domain-security
source_filename: branchtechnology-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-03'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: branchtechnology.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 11 03:14:29 2026 GMT\n  hsts: false\ndomains:\n- domain: branchtechnology.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/branchtechnology/refs/heads/main/security/branchtechnology-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- 3D Printing
- Construction Tech
- Additive Manufacturing
- SpaceIndustry
---
