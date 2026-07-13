---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: boeing.com
  spf: true
hosts:
- cert_expires: Jan  1 23:59:59 2027 GMT
  host: www.boeing.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  5 23:59:59 2026 GMT
  host: developer.boeing.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Boeing Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Boeing, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Boeing
provider_slug: boeing
slug: boeing-domain-security
source_filename: boeing-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.boeing.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  1 23:59:59 2027 GMT\n  hsts: false\n- host: developer.boeing.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  5 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: boeing.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/boeing/refs/heads/main/security/boeing-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Aviation
- Airplanes
- Aerospace
- Flight
- Aeronautical
- Fortune 100
---
