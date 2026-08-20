---
api_specs:
- filename: pavoot-api-openapi.json
  format: json
  label: Pavoot Application API
  slug: pavoot-application-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pavoot/refs/heads/main/openapi/pavoot-api-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: pavoot.com
  spf: true
hosts:
- cert_expires: Oct 21 05:12:44 2026 GMT
  host: pavoot.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Pavoot Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Pavoot, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Pavoot
provider_slug: pavoot
slug: pavoot-domain-security
source_filename: pavoot-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: pavoot.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 21 05:12:44 2026 GMT\n  hsts: false\ndomains:\n- domain: pavoot.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pavoot/refs/heads/main/security/pavoot-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Event
- Event Management
- Marketing
- AI Agent
- Attendee Intelligence
- Go-To-Market
- Field Marketing
- Pipeline
---
