---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: geobytes.com
  spf: true
hosts:
- cert_expires: Jan  7 05:52:01 2027 GMT
  host: geobytes.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Geobytes Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Geobytes, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Geobytes
provider_slug: geobytes
slug: geobytes-domain-security
source_filename: geobytes-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: geobytes.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  7 05:52:01 2027 GMT\n  hsts: false\ndomains:\n- domain: geobytes.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/geobytes/security/geobytes-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Geolocation
- IP
- API
- Free
---
