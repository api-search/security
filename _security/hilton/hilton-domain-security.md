---
api_specs:
- filename: hilton-hilton-api-openapi.yml
  format: yaml
  label: Hilton Developer API
  slug: hilton-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hilton/refs/heads/main/openapi/hilton-hilton-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: hilton.com
  spf: true
hosts:
- cert_expires: Aug 14 23:59:59 2026 GMT
  host: www.hilton.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- host: developer.hilton.com
  https: false
- host: api.hilton.com
  https: false
kind: domain-security
layout: security
method: probed
name: Hilton Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Hilton, probed live across 3 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Hilton
provider_slug: hilton
slug: hilton-domain-security
source_filename: hilton-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.hilton.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 14 23:59:59 2026 GMT\n  hsts: null\n- host: developer.hilton.com\n  https: false\n- host: api.hilton.com\n  https: false\ndomains:\n- domain: hilton.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hilton/refs/heads/main/security/hilton-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Hospitality
- Hotels
- Travel
- Reservations
- Loyalty
---
