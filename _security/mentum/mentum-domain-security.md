---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: true
  domain: getmentum.com
  spf: true
hosts:
- cert_expires: Jan 15 08:18:12 2027 GMT
  host: getmentum.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Mentum Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Mentum, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC absent.'
provider_name: Mentum
provider_slug: mentum
slug: mentum-domain-security
source_filename: mentum-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: getmentum.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 15 08:18:12 2027 GMT\n  hsts: null\ndomains:\n- domain: getmentum.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/mentum/security/mentum-domain-security.yml
summary_line: TLSv1.3 · DNSSEC
tags:
- Company
- Startup
- FinTech
- API
- VentureBacked
---
