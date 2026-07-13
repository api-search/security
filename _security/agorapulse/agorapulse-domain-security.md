---
api_specs:
- filename: open-api.yml
  format: yaml
  label: Agorapulse Reports Open API
  slug: agorapulse-reports-api
  spec_type: OpenAPI
  url: https://api.agorapulse.com/docs/open-api.yml
description: ''
domains:
- caa:
  - 0 issue "amazonaws.com"
  - 0 issue "letsencrypt.org"
  - 0 issuewild "amazonaws.com"
  dmarc: false
  dnssec: false
  domain: agorapulse.com
  spf: true
hosts:
- cert_expires: Nov  4 23:59:59 2026 GMT
  host: www.agorapulse.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 15 23:59:59 2026 GMT
  host: support.agorapulse.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec  4 23:59:59 2026 GMT
  host: api.agorapulse.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Agorapulse Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Agorapulse, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Agorapulse
provider_slug: agorapulse
slug: agorapulse-domain-security
source_filename: agorapulse-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.agorapulse.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  4 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: support.agorapulse.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 23:59:59 2026 GMT\n  hsts: false\n- host: api.agorapulse.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  4 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: agorapulse.com\n  dnssec: false\n  caa:\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issuewild \"amazonaws.com\"\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/agorapulse/refs/heads/main/security/agorapulse-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Social Media Management
- Social Media
- CRM
- Analytics
- Publishing
- Inbox Management
- Social Listening
---
