---
api_specs:
- filename: steelcase-roomwizard-api-openapi.yml
  format: yaml
  label: Steelcase RoomWizard API
  slug: roomwizard-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/steelcase/refs/heads/main/openapi/steelcase-roomwizard-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: steelcase.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: roomwizard.local
  spf: false
hosts:
- cert_expires: Aug 31 23:59:59 2026 GMT
  host: www.steelcase.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- host: roomwizard.local
  https: false
kind: domain-security
layout: security
method: probed
name: Steelcase Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Steelcase, probed live across 2 host(s) and 2 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Steelcase
provider_slug: steelcase
slug: steelcase-domain-security
source_filename: steelcase-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.steelcase.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 31 23:59:59 2026 GMT\n  hsts: false\n- host: roomwizard.local\n  https: false\ndomains:\n- domain: steelcase.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: roomwizard.local\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/steelcase/refs/heads/main/security/steelcase-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Office Furniture
- Workplace
- Room Scheduling
- Facilities Management
- IoT
- Smart Office
- Fortune 1000
---
