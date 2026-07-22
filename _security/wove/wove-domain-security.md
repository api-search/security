---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: wove.com
  spf: true
hosts:
- cert_expires: Sep 10 01:59:57 2026 GMT
  host: wove.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 26 04:46:32 2026 GMT
  host: api.wove.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- host: staging-api.wove.com
  https: false
kind: domain-security
layout: security
method: probed
name: Wove Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Wove, probed live across 3 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Wove
provider_slug: wove
slug: wove-domain-security
source_filename: wove-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: wove.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 10 01:59:57 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.wove.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 26 04:46:32 2026 GMT\n  hsts: null\n- host: staging-api.wove.com\n  https: false\ndomains:\n- domain: wove.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wove/refs/heads/main/security/wove-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
---
