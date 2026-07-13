---
api_specs:
- filename: realtor-connections-plus-asyncapi.yml
  format: yaml
  label: Realtor.com Connections Plus API
  slug: connections-plus-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/realtor/refs/heads/main/asyncapi/realtor-connections-plus-asyncapi.yml
- filename: realtor-lead-delivery-asyncapi.yml
  format: yaml
  label: Realtor.com Lead Delivery API
  slug: lead-delivery-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/realtor/refs/heads/main/asyncapi/realtor-lead-delivery-asyncapi.yml
- filename: realtor-property-data-openapi.yml
  format: yaml
  label: Realtor.com Property Data API
  slug: property-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/realtor/refs/heads/main/openapi/realtor-property-data-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: realtor.com
  spf: true
- caa: []
  dmarc: false
  dnssec: true
  domain: rapidapi.com
  spf: true
hosts:
- cert_expires: Dec  3 23:59:59 2026 GMT
  host: www.realtor.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 18 08:42:50 2026 GMT
  host: rapidapi.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 18 23:59:59 2026 GMT
  host: realtor.p.rapidapi.com
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Realtor Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for realtor, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: realtor
provider_slug: realtor
slug: realtor-domain-security
source_filename: realtor-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.realtor.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  3 23:59:59 2026 GMT\n  hsts: null\n- host: rapidapi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 18 08:42:50 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: realtor.p.rapidapi.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep 18 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: realtor.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: rapidapi.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/realtor/refs/heads/main/security/realtor-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags: []
---
