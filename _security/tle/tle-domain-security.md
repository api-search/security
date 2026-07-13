---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: ivanstanojevic.me
  spf: true
hosts:
- cert_expires: Sep  2 21:12:25 2026 GMT
  host: tle.ivanstanojevic.me
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Tle Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for TLE, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: TLE
provider_slug: tle
slug: tle-domain-security
source_filename: tle-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: tle.ivanstanojevic.me\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  2 21:12:25 2026 GMT\n  hsts: null\ndomains:\n- domain: ivanstanojevic.me\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tle/refs/heads/main/security/tle-domain-security.yml
summary_line: TLSv1.3
tags:
- Science And Math
- Public APIs
---
