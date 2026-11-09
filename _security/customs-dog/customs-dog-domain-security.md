---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: customs.dog
  spf: true
hosts:
- cert_expires: Jan  1 19:28:14 2027 GMT
  host: customs.dog
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Customs Dog Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for customs.dog, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: customs.dog
provider_slug: customs-dog
slug: customs-dog-domain-security
source_filename: customs-dog-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: customs.dog\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  1 19:28:14 2027 GMT\n  hsts: false\ndomains:\n- domain: customs.dog\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/customs-dog/security/customs-dog-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Pet travel
- Border crossing
- Customs
- Travel app
---
