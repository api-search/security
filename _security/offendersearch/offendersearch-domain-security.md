---
api_specs:
- filename: openapi.json
  format: json
  label: Offendersearch API
  slug: offendersearch-api
  spec_type: OpenAPI
  url: https://offendersearch.app/openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: offendersearch.app
  spf: true
hosts:
- cert_expires: Oct 27 13:39:50 2026 GMT
  host: offendersearch.app
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 27 13:39:03 2026 GMT
  host: api.offendersearch.app
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 2
kind: domain-security
layout: security
method: probed
name: Offendersearch Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Offendersearch, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Offendersearch
provider_slug: offendersearch
slug: offendersearch-domain-security
source_filename: offendersearch-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-03'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: offendersearch.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 27 13:39:50 2026 GMT\n  hsts: false\n- host: api.offendersearch.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 27 13:39:03 2026 GMT\n  hsts: null\ndomains:\n- domain: offendersearch.app\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/offendersearch/refs/heads/main/security/offendersearch-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Background Screening
- Identity & risk
- Trust and Safety
- Public Records
- Criminal data
- Compliance
- Sex-offender registry data
- Staffing & recruiting
- Tenant Screening
- Healthcare
- Gig marketplaces
---
