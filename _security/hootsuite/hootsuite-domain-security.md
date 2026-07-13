---
api_specs:
- filename: hootsuite-openapi.yml
  format: yaml
  label: Hootsuite REST API
  slug: rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hootsuite/refs/heads/main/openapi/hootsuite-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "cloudflare.com"
  - 0 issue "cloudflaressl.com"
  - 0 issue "comodo.com"
  - 0 issue "digicert.com"
  - 0 issue "godaddy.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: hootsuite.com
  spf: true
hosts:
- cert_expires: Sep 24 04:24:36 2026 GMT
  host: www.hootsuite.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  3 11:28:58 2026 GMT
  host: developer.hootsuite.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 17 23:59:59 2026 GMT
  host: platform.hootsuite.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Hootsuite Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Hootsuite, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Hootsuite
provider_slug: hootsuite
slug: hootsuite-domain-security
source_filename: hootsuite-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.hootsuite.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 24 04:24:36 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developer.hootsuite.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 11:28:58 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: platform.hootsuite.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 17 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: hootsuite.com\n  dnssec: false\n  caa:\n  - 0 issue \"cloudflare.com\"\n  - 0 issue \"cloudflaressl.com\"\n  - 0 issue \"comodo.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"godaddy.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hootsuite/refs/heads/main/security/hootsuite-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Social Media
- Social Media Management
- Marketing
- Content Scheduling
- Analytics
- Engagement
---
