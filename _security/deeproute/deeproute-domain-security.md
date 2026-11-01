---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: deeproute.tech
  spf: false
hosts:
- cert_expires: Jan  7 22:35:08 2027 GMT
  host: www.deeproute.tech
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Deeproute Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Deeproute, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Deeproute
provider_slug: deeproute
slug: deeproute-domain-security
source_filename: deeproute-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-22'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.deeproute.tech\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  7 22:35:08 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: deeproute.tech\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/deeproute/security/deeproute-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Outreach
- Sports
- Recruiting
- Education
---
