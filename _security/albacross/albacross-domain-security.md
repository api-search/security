---
api_specs:
- filename: albacross-reveal-openapi.yml
  format: yaml
  label: Albacross Reveal API
  slug: albacross-reveal-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/albacross/refs/heads/main/openapi/albacross-reveal-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: albacross.com
  spf: true
hosts:
- cert_expires: Oct 20 18:24:58 2026 GMT
  host: albacross.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  8 23:59:59 2026 GMT
  host: docs.albacross.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb 16 23:59:59 2027 GMT
  host: api.albacross.com
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Albacross Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Albacross, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Albacross
provider_slug: albacross
slug: albacross-domain-security
source_filename: albacross-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: albacross.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 20 18:24:58 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.albacross.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  8 23:59:59 2026 GMT\n  hsts: false\n- host: api.albacross.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Feb 16 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: albacross.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/albacross/refs/heads/main/security/albacross-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- B2B Data
- Lead Generation
- Intent Data
- Company Enrichment
- IP Intelligence
- Firmographics
- Marketing
- Sales Intelligence
- Account Based Marketing
- Website Visitor Identification
- Webhooks
---
