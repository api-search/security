---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: intrinio.com
  spf: true
hosts:
- cert_expires: Sep 15 21:05:26 2026 GMT
  host: intrinio.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Intrinio Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Intrinio, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Intrinio
provider_slug: intrinio
slug: intrinio-domain-security
source_filename: intrinio-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: intrinio.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 21:05:26 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: intrinio.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/intrinio/refs/heads/main/security/intrinio-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Finance
- Public APIs
---
