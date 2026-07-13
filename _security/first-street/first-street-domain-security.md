---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: firststreet.org
  spf: true
hosts:
- cert_expires: Dec 10 23:59:59 2026 GMT
  host: firststreet.org
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  1 06:02:00 2026 GMT
  host: docs.firststreet.org
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 10 23:59:59 2026 GMT
  host: api.firststreet.org
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: First Street Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for First Street, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: First Street
provider_slug: first-street
slug: first-street-domain-security
source_filename: first-street-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: firststreet.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 10 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.firststreet.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  1 06:02:00 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.firststreet.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 10 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: firststreet.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/first-street/refs/heads/main/security/first-street-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Environment
- Modeling
- Risk
- Climate
---
