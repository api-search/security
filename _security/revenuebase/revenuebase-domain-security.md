---
api_specs:
- filename: revenuebase-openapi.json
  format: json
  label: Revenuebase API v2
  slug: revenuebase-api-v2
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/revenuebase/refs/heads/main/openapi/revenuebase-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: revenuebase.ai
  spf: true
hosts:
- cert_expires: Sep  9 16:45:33 2026 GMT
  host: revenuebase.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 24 23:59:59 2026 GMT
  host: api.revenuebase.ai
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Revenuebase Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for RevenueBase, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: RevenueBase
provider_slug: revenuebase
slug: revenuebase-domain-security
source_filename: revenuebase-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: revenuebase.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  9 16:45:33 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.revenuebase.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 24 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: revenuebase.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/revenuebase/refs/heads/main/security/revenuebase-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- B2B Data
- Data Enrichment
- Email Verification
- Contact Data
- Company Data
- Lead Intelligence
- Sales Intelligence
---
