---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: nesimplicity.com
  spf: true
hosts:
- cert_expires: Jan 22 04:48:10 2027 GMT
  host: nesimplicity.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: SimpliCity Real Estate Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for SimpliCity Real Estate, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: SimpliCity Real Estate
provider_slug: nesimplicity-com
slug: nesimplicity-com-domain-security
source_filename: nesimplicity-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: nesimplicity.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 22 04:48:10 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: nesimplicity.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/nesimplicity-com/security/nesimplicity-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Real Estate
- Agency
- Lincoln
- Nebraska
- VAloans
- Home Buying
---
