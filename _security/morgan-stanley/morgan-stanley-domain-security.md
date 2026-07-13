---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: morganstanley.com
  spf: true
hosts:
- cert_expires: Jan 21 23:59:59 2027 GMT
  host: developer.morganstanley.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Morgan Stanley Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Morgan Stanley, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Morgan Stanley
provider_slug: morgan-stanley
slug: morgan-stanley-domain-security
source_filename: morgan-stanley-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developer.morganstanley.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 21 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: morganstanley.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/morgan-stanley/refs/heads/main/security/morgan-stanley-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Financial
- Investment Banking
- Wealth Management
- Fortune 100
---
