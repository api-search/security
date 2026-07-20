---
api_specs:
- filename: kolide-k2-openapi.json
  format: json
  label: Kolide K2 API
  slug: kolide-k2-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kolide/refs/heads/main/openapi/kolide-k2-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: kolide.com
  spf: true
hosts:
- cert_expires: Nov  4 23:59:59 2026 GMT
  host: kolide.com
  hsts: true
  hsts_max_age: 631138519
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  4 23:59:59 2026 GMT
  host: api.kolide.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Kolide Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Kolide, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Kolide
provider_slug: kolide
slug: kolide-domain-security
source_filename: kolide-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: kolide.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  4 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 631138519\n- host: api.kolide.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  4 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: kolide.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kolide/refs/heads/main/security/kolide-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- B2B
- Security
- Device Trust
- Endpoint Security
- Zero Trust
- Compliance
- Identity
- osquery
- Device Management
---
