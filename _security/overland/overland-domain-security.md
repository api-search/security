---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: p3k.app
  spf: false
hosts:
- cert_expires: Jan  8 10:16:13 2027 GMT
  host: overland.p3k.app
  hsts: false
  https: true
  tls_version: TLSv1.2
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Overland Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Overland, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Overland
provider_slug: overland
slug: overland-domain-security
source_filename: overland-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: overland.p3k.app\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jan  8 10:16:13 2027 GMT\n  hsts: false\ndomains:\n- domain: p3k.app\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/overland/security/overland-domain-security.yml
summary_line: TLSv1.2
tags:
- GPS
- OpenSource
- iOS
- LocationTracking
- Privacy
---
