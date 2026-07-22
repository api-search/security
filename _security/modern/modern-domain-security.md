---
api_specs:
- filename: modern-partner-api-openapi.yml
  format: yaml
  label: MODERN Partner API
  slug: modern-partner-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/modern/refs/heads/main/openapi/modern-partner-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: modernis.com
  spf: true
hosts:
- cert_expires: Oct 11 18:48:52 2026 GMT
  host: modernis.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Modern Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Modern, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Modern
provider_slug: modern
slug: modern-domain-security
source_filename: modern-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: modernis.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 11 18:48:52 2026 GMT\n  hsts: false\ndomains:\n- domain: modernis.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/modern/refs/heads/main/security/modern-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Heavy Equipment
- Dealership
- Field Service
- Work Orders
- Customer Communications
- Notifications
- Partner API
---
