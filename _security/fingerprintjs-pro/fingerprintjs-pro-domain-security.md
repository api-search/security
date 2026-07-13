---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: fingerprintjs.com
  spf: true
hosts:
- cert_expires: Mar 19 23:59:59 2027 GMT
  host: dev.fingerprintjs.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Fingerprintjs Pro Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for FingerprintJS Pro, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: FingerprintJS Pro
provider_slug: fingerprintjs-pro
slug: fingerprintjs-pro-domain-security
source_filename: fingerprintjs-pro-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: dev.fingerprintjs.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 19 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: fingerprintjs.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fingerprintjs-pro/refs/heads/main/security/fingerprintjs-pro-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Security
- Public APIs
---
