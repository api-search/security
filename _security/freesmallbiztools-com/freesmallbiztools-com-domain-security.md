---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: freesmallbiztools.com
  spf: true
hosts:
- cert_expires: Jan 12 12:39:13 2027 GMT
  host: freesmallbiztools.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Free Small Biz Tools Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Free Small Biz Tools, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Free Small Biz Tools
provider_slug: freesmallbiztools-com
slug: freesmallbiztools-com-domain-security
source_filename: freesmallbiztools-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-08'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: freesmallbiztools.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 12 12:39:13 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: freesmallbiztools.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/freesmallbiztools-com/security/freesmallbiztools-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Directory
- Small Business
- Omaha
- Open Source
---
