---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: true
  domain: mechoulam.de
  spf: false
hosts:
- cert_expires: Jan  4 17:30:48 2027 GMT
  host: mechoulam.de
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Mechoulam Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Mechoulam, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF absent, DMARC absent.'
provider_name: Mechoulam
provider_slug: mechoulam-de
slug: mechoulam-de-domain-security
source_filename: mechoulam-de-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: mechoulam.de\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  4 17:30:48 2027 GMT\n  hsts: null\ndomains:\n- domain: mechoulam.de\n  dnssec: true\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/mechoulam-de/security/mechoulam-de-domain-security.yml
summary_line: TLSv1.3 · DNSSEC
tags:
- Cannabis
- Research
- Healthcare
- Data
- Open Source
---
