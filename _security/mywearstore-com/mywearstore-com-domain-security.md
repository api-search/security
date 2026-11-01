---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: mywearstore.com
  spf: true
hosts:
- cert_expires: Dec 25 11:19:59 2026 GMT
  host: www.mywearstore.com
  hsts: false
  https: true
  tls_version: TLSv1.2
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Mywearstore Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for MyWear, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: MyWear
provider_slug: mywearstore-com
slug: mywearstore-com-domain-security
source_filename: mywearstore-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-25'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.mywearstore.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec 25 11:19:59 2026 GMT\n  hsts: false\ndomains:\n- domain: mywearstore.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/mywearstore-com/security/mywearstore-com-domain-security.yml
summary_line: TLSv1.2
tags:
- Company
---
