---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: littlegreenlight.com
  spf: true
hosts:
- cert_expires: Apr  2 23:59:59 2027 GMT
  host: littlegreenlight.com
  hsts: false
  https: true
  tls_version: TLSv1.2
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Little Green Light Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Little Green Light, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Little Green Light
provider_slug: little-green-light
slug: little-green-light-domain-security
source_filename: little-green-light-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-27'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: littlegreenlight.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Apr  2 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: littlegreenlight.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/little-green-light/security/little-green-light-domain-security.yml
summary_line: TLSv1.2 · DMARC
tags:
- Donor Management
- Nonprofit Software
- Fundraising
- Online Donations
- Data Management
---
