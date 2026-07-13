---
api_specs:
- filename: uplead-openapi.json
  format: json
  label: UpLead API
  slug: uplead-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uplead/refs/heads/main/openapi/uplead-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: uplead.com
  spf: true
hosts:
- cert_expires: Aug 13 23:31:54 2026 GMT
  host: www.uplead.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 13 23:31:54 2026 GMT
  host: docs.uplead.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 13 23:31:54 2026 GMT
  host: api.uplead.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Uplead Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for UpLead, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: UpLead
provider_slug: uplead
slug: uplead-domain-security
source_filename: uplead-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.uplead.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 13 23:31:54 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.uplead.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 13 23:31:54 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.uplead.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 13 23:31:54 2026 GMT\n  hsts: null\ndomains:\n- domain: uplead.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/uplead/refs/heads/main/security/uplead-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- B2B
- Lead Generation
- Contact Data
- Company Data
- Email Verification
- Data Enrichment
- Sales Intelligence
---
