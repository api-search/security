---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: ncstatutes.com
  spf: true
hosts:
- cert_expires: Jan 11 18:49:43 2027 GMT
  host: ncstatutes.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: SmartBump, Inc. Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for SmartBump, Inc., probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: SmartBump, Inc.
provider_slug: ncstatutes-com
slug: ncstatutes-com-domain-security
source_filename: ncstatutes-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ncstatutes.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 11 18:49:43 2027 GMT\n  hsts: false\ndomains:\n- domain: ncstatutes.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/ncstatutes-com/security/ncstatutes-com-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Legal Tech
- Artificial Intelligence
- Law
- North Carolina
- Open Data
---
