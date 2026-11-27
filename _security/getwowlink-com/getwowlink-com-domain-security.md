---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: getwowlink.com
  spf: true
hosts:
- cert_expires: Jan 12 23:31:52 2027 GMT
  host: getwowlink.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: getwowlink Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for getwowlink, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: getwowlink
provider_slug: getwowlink-com
slug: getwowlink-com-domain-security
source_filename: getwowlink-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-10'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: getwowlink.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 12 23:31:52 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: getwowlink.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/getwowlink-com/security/getwowlink-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- OpenGraph
- Web Integration
- SaaS Tools
---
