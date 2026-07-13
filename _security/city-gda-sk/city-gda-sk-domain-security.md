---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: multimediagdansk.pl
  spf: false
hosts:
- cert_expires: Jul 19 10:17:23 2026 GMT
  host: ckan.multimediagdansk.pl
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: City Gda Sk Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for City, Gdańsk, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: City, Gdańsk
provider_slug: city-gda-sk
slug: city-gda-sk-domain-security
source_filename: city-gda-sk-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ckan.multimediagdansk.pl\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jul 19 10:17:23 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: multimediagdansk.pl\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/city-gda-sk/refs/heads/main/security/city-gda-sk-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Government
- Public APIs
---
