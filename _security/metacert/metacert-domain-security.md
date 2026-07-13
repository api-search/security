---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: metacert.com
  spf: true
hosts:
- cert_expires: Aug 16 06:21:05 2026 GMT
  host: metacert.com
  hsts: true
  hsts_max_age: 10886400
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Metacert Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Metacert, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Metacert
provider_slug: metacert
slug: metacert-domain-security
source_filename: metacert-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: metacert.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 16 06:21:05 2026 GMT\n  hsts: true\n  hsts_max_age: 10886400\ndomains:\n- domain: metacert.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/metacert/refs/heads/main/security/metacert-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Anti Malware
- Public APIs
---
