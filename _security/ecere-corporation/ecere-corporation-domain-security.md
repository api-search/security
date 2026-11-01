---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: ecere.ca
  spf: true
hosts:
- cert_expires: Jan  9 17:35:49 2027 GMT
  host: ecere.ca
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Ecere Corporation Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Ecere Corporation, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Ecere Corporation
provider_slug: ecere-corporation
slug: ecere-corporation-domain-security
source_filename: ecere-corporation-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ecere.ca\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  9 17:35:49 2027 GMT\n  hsts: false\ndomains:\n- domain: ecere.ca\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/ecere-corporation/security/ecere-corporation-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Graphics
- Software
- SDK
- Development
---
