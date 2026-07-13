---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: nordson.com
  spf: true
hosts:
- cert_expires: Oct  7 01:12:28 2026 GMT
  host: www.nordson.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- host: developer.nordson.com
  https: false
- host: api.nordson.com
  https: false
kind: domain-security
layout: security
method: probed
name: Nordson Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Nordson Corporation, probed live across 3 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Nordson Corporation
provider_slug: nordson
slug: nordson-domain-security
source_filename: nordson-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.nordson.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  7 01:12:28 2026 GMT\n  hsts: null\n- host: developer.nordson.com\n  https: false\n- host: api.nordson.com\n  https: false\ndomains:\n- domain: nordson.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nordson/refs/heads/main/security/nordson-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Dispensing
- Testing
- Industrial
---
