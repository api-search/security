---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: adace.website
  spf: true
hosts:
- cert_expires: Jan 28 12:29:12 2027 GMT
  host: adace.website
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Adace Website Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AdAce, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: AdAce
provider_slug: adace-website
slug: adace-website-domain-security
source_filename: adace-website-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: adace.website\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 28 12:29:12 2027 GMT\n  hsts: false\ndomains:\n- domain: adace.website\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/adace-website/security/adace-website-domain-security.yml
summary_line: TLSv1.3
tags:
- Advertising
- Lead Generation
- Marketing
- Software-as-a-Service
- Agency
---
