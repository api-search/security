---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: charitymiles.org
  spf: true
hosts:
- cert_expires: Apr  5 11:24:08 2027 GMT
  host: charitymiles.org
  hsts: false
  https: true
  tls_version: TLSv1.2
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Charity Miles Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Charity Miles, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Charity Miles
provider_slug: charity-miles
slug: charity-miles-domain-security
source_filename: charity-miles-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-27'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: charitymiles.org\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Apr  5 11:24:08 2027 GMT\n  hsts: false\ndomains:\n- domain: charitymiles.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/charity-miles/security/charity-miles-domain-security.yml
summary_line: TLSv1.2 · DMARC
tags:
- Company
- Fitness
- Charity
- MobileApp
- Health
---
