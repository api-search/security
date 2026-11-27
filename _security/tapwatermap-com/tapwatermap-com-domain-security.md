---
description: ''
domains:
- caa: []
  dmarc: false
  dns_aid:
    checked: '2026-11-26'
    published: false
  dnssec: false
  domain: tapwatermap.com
  spf: false
hosts:
- cert_expires: Jan 11 21:06:27 2027 GMT
  host: tapwatermap.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: TapWaterMap Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for TapWaterMap, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: TapWaterMap
provider_slug: tapwatermap-com
slug: tapwatermap-com-domain-security
source_filename: tapwatermap-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: tapwatermap.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 11 21:06:27 2027 GMT\n  hsts: false\ndomains:\n- domain: tapwatermap.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n  dns_aid:\n    checked: '2026-11-26'\n    published: false\n"
source_yaml_url: https://artifacts.apis.io/tapwatermap-com/security/tapwatermap-com-domain-security.yml
summary_line: TLSv1.3
tags:
- Water
- Data
- EPA
- PublicHealth
- API
---
