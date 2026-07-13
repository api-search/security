---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: saia.com
  spf: true
hosts:
- cert_expires: Sep 30 14:45:52 2026 GMT
  host: www.saia.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- host: developer.saia.com
  https: false
- cert_expires: Oct 31 23:59:59 2026 GMT
  host: api.saia.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Saia Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Saia Inc, probed live across 3 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Saia Inc
provider_slug: saia
slug: saia-domain-security
source_filename: saia-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.saia.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 14:45:52 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developer.saia.com\n  https: false\n- host: api.saia.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 31 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: saia.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/saia/refs/heads/main/security/saia-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Freight
- Trucking
- Logistics
---
