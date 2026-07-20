---
api_specs:
- filename: govly-tools-v1-openapi-original.yml
  format: yaml
  label: Govly Tools API
  slug: govly-tools-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/govly/refs/heads/main/openapi/govly-tools-v1-openapi-original.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: govly.com
  spf: true
hosts:
- cert_expires: Oct 14 15:05:37 2026 GMT
  host: www.govly.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 31 06:05:43 2026 GMT
  host: docs.govly.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  2 08:43:52 2026 GMT
  host: app.govly.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Govly Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Govly, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Govly
provider_slug: govly
slug: govly-domain-security
source_filename: govly-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.govly.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 14 15:05:37 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.govly.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 31 06:05:43 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: app.govly.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  2 08:43:52 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: govly.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/govly/refs/heads/main/security/govly-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Government
- Public Sector
- Procurement
- Government Contracting
- GovTech
- Market Intelligence
- Awards
- Opportunities
- Agents
---
