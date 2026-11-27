---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: daall.sa
  spf: true
hosts:
- cert_expires: Jan  3 11:14:51 2027 GMT
  host: daall.sa
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: دال Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for دال, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: دال
provider_slug: daall-sa
slug: daall-sa-domain-security
source_filename: daall-sa-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: daall.sa\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  3 11:14:51 2027 GMT\n  hsts: false\ndomains:\n- domain: daall.sa\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/daall-sa/security/daall-sa-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Data Analytics
- Government
- Saudi Arabia
- Market Research
---
