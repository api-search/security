---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: firstlook.biz
  spf: false
hosts:
- cert_expires: Mar  1 23:59:59 2027 GMT
  host: firstlook.biz
  hsts: true
  hsts_max_age: 15768000
  https: true
  tls_version: TLSv1.2
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: FirstLook Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for FirstLook, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: FirstLook
provider_slug: firstlook
slug: firstlook-domain-security
source_filename: firstlook-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-16'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: firstlook.biz\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Mar  1 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 15768000\ndomains:\n- domain: firstlook.biz\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/firstlook/security/firstlook-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Company
---
