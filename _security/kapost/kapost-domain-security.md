---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: kapost.com
  spf: true
hosts:
- cert_expires: Feb 16 23:59:59 2027 GMT
  host: kapost.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
- cert_expires: Dec 18 11:11:18 2026 GMT
  host: developer.kapost.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 18 11:11:18 2026 GMT
  host: api.kapost.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Kapost Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Kapost, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.2); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Kapost
provider_slug: kapost
slug: kapost-domain-security
source_filename: kapost-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: kapost.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Feb 16 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developer.kapost.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 18 11:11:18 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.kapost.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 18 11:11:18 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: kapost.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kapost/refs/heads/main/security/kapost-domain-security.yml
summary_line: TLSv1.2 · HSTS
tags:
- Content Operations
- Content Marketing
- Content Management
- Marketing
- Sales Enablement
- Webhook
- REST API
- B2B
- Upland Software
---
