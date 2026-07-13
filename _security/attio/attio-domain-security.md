---
api_specs:
- filename: openapi
  format: yaml
  label: Attio REST API
  slug: rest-api
  spec_type: OpenAPI
  url: https://docs.attio.com/rest-api/endpoint-reference/openapi
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: attio.com
  spf: true
hosts:
- cert_expires: Jul 28 04:13:19 2026 GMT
  host: attio.com
  hsts: true
  hsts_max_age: 7776000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 31 13:50:40 2026 GMT
  host: docs.attio.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jul 28 04:13:19 2026 GMT
  host: api.attio.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Attio Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Attio, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Attio
provider_slug: attio
slug: attio-domain-security
source_filename: attio-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: attio.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jul 28 04:13:19 2026 GMT\n  hsts: true\n  hsts_max_age: 7776000\n- host: docs.attio.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 31 13:50:40 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.attio.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jul 28 04:13:19 2026 GMT\n  hsts: null\ndomains:\n- domain: attio.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/attio/refs/heads/main/security/attio-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- CRM
- Customer Relationship Management
- Sales
- Contacts
- Companies
- Pipeline
- Workflows
---
