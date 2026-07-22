---
api_specs:
- filename: ntropy-api-v3-openapi-original.json
  format: json
  label: Ntropy Transaction API (v3)
  slug: ntropy-transaction-api-v3
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ntropy/refs/heads/main/openapi/ntropy-api-v3-openapi-original.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: ntropy.network
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: ntropy.com
  spf: true
hosts:
- cert_expires: Aug 22 22:45:16 2026 GMT
  host: ntropy.network
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 30 14:59:23 2026 GMT
  host: api.ntropy.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Ntropy Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Ntropy, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Ntropy
provider_slug: ntropy
slug: ntropy-domain-security
source_filename: ntropy-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ntropy.network\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 22 22:45:16 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.ntropy.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 30 14:59:23 2026 GMT\n  hsts: null\ndomains:\n- domain: ntropy.network\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: ntropy.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ntropy/refs/heads/main/security/ntropy-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Fintech
- Transaction Enrichment
- Financial Data
- Data Enrichment
- Bank Statements
- Categorization
- Underwriting
---
