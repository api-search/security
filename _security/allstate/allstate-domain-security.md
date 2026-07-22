---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: allstate.com
  spf: true
hosts:
- cert_expires: Sep  6 23:59:59 2026 GMT
  host: www.allstate.com
  hsts: true
  hsts_max_age: 15768000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  3 23:59:59 2026 GMT
  host: developer.allstate.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Allstate Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Allstate, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Allstate
provider_slug: allstate
slug: allstate-domain-security
source_filename: allstate-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.allstate.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  6 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 15768000\n- host: developer.allstate.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Nov  3 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: allstate.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/allstate/refs/heads/main/security/allstate-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Insurance
- Auto Insurance
- Home Insurance
- Life Insurance
- Personal Lines
---
