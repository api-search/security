---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: fatestar.top
  spf: true
hosts:
- cert_expires: Feb  3 05:19:37 2027 GMT
  host: fatestar.top
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Fatestar Top Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for FateStar, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: FateStar
provider_slug: fatestar-top
slug: fatestar-top-domain-security
source_filename: fatestar-top-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-07'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: fatestar.top\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  3 05:19:37 2027 GMT\n  hsts: false\ndomains:\n- domain: fatestar.top\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/fatestar-top/security/fatestar-top-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
---
