---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: codelco.com
  spf: false
hosts:
- cert_expires: Mar 10 23:59:59 2027 GMT
  host: www.codelco.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Codelco Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Codelco, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Codelco
provider_slug: codelco
slug: codelco-domain-security
source_filename: codelco-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.codelco.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 10 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: codelco.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/codelco/security/codelco-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Mining
- Copper
- Chile
- State-Owned Enterprise
- Natural Resources
---
