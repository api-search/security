---
api_specs:
- filename: unify-data-openapi.json
  format: json
  label: Unify Data API
  slug: unify-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unify/refs/heads/main/openapi/unify-data-openapi.json
- filename: unify-sequences-openapi.json
  format: json
  label: Unify Sequences API
  slug: unify-sequences-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unify/refs/heads/main/openapi/unify-sequences-openapi.json
- filename: unify-analytics-openapi.json
  format: json
  label: Unify Analytics API
  slug: unify-analytics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unify/refs/heads/main/openapi/unify-analytics-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: unifygtm.com
  spf: true
hosts:
- cert_expires: Sep 12 12:54:01 2026 GMT
  host: www.unifygtm.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 21 11:27:59 2026 GMT
  host: docs.unifygtm.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 27 23:59:59 2026 GMT
  host: api.unifygtm.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Unify Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Unify, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Unify
provider_slug: unify
slug: unify-domain-security
source_filename: unify-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.unifygtm.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 12 12:54:01 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.unifygtm.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 21 11:27:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.unifygtm.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 27 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: unifygtm.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/unify/refs/heads/main/security/unify-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Sales
- Marketing
- Go-To-Market
- Outbound
- Intent Data
- AI Agents
- B2B
- Data Enrichment
- Sequences
- Analytics
---
