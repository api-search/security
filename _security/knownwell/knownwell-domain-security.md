---
api_specs:
- filename: knownwell-ci-openapi-original.json
  format: json
  label: Knownwell API
  slug: knownwell-ci
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/knownwell/refs/heads/main/openapi/knownwell-ci-openapi-original.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: knownwell.com
  spf: true
hosts:
- cert_expires: Oct 14 16:46:48 2026 GMT
  host: knownwell.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 24 12:22:59 2026 GMT
  host: api.knownwell.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Knownwell Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Knownwell, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Knownwell
provider_slug: knownwell
slug: knownwell-domain-security
source_filename: knownwell-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: knownwell.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 14 16:46:48 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.knownwell.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 24 12:22:59 2026 GMT\n  hsts: null\ndomains:\n- domain: knownwell.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/knownwell/refs/heads/main/security/knownwell-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Commercial Intelligence
- Client Intelligence
- Customer Success
- Revenue Operations
- Professional Services
- Artificial Intelligence
- Analytics
- CRM
- Churn Risk
---
