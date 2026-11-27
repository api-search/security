---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: d.cv
  spf: false
hosts:
- cert_expires: Jan 27 13:17:31 2027 GMT
  host: d.cv
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: d-cv Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for d-cv, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: d-cv
provider_slug: d-cv
slug: d-cv-domain-security
source_filename: d-cv-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: d.cv\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 27 13:17:31 2027 GMT\n  hsts: null\ndomains:\n- domain: d.cv\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/d-cv/security/d-cv-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
---
