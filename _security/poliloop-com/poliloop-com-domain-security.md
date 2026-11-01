---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: poliloop.com
  spf: true
hosts:
- cert_expires: Jan  2 22:23:35 2027 GMT
  host: poliloop.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Poliloop Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for PolyXLabs, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: PolyXLabs
provider_slug: poliloop-com
slug: poliloop-com-domain-security
source_filename: poliloop-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-24'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: poliloop.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  2 22:23:35 2027 GMT\n  hsts: null\ndomains:\n- domain: poliloop.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/poliloop-com/security/poliloop-com-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Polymer
- Materials
- API
- Sustainability
- Aerospace
---
