---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: aeralas.com
  spf: true
hosts:
- cert_expires: Jan 21 17:57:44 2027 GMT
  host: aeralas.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Aeralas Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for aeralas-com, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: aeralas-com
provider_slug: aeralas-com
slug: aeralas-com-domain-security
source_filename: aeralas-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-01'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: aeralas.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 21 17:57:44 2027 GMT\n  hsts: null\ndomains:\n- domain: aeralas.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/aeralas-com/security/aeralas-com-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
---
