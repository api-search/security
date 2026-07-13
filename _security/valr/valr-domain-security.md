---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: valr.com
  spf: true
hosts:
- cert_expires: Sep 17 23:57:19 2026 GMT
  host: docs.valr.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Valr Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for VALR, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: VALR
provider_slug: valr
slug: valr-domain-security
source_filename: valr-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: docs.valr.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 17 23:57:19 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: valr.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/valr/refs/heads/main/security/valr-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Cryptocurrency
- Public APIs
---
