---
api_specs:
- filename: dhl-openapi.yml
  format: yaml
  label: Location Finder Unified
  slug: location-finder-unified
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dhl/refs/heads/main/openapi/dhl-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: dhl.com
  spf: true
hosts:
- cert_expires: Oct 31 04:01:35 2026 GMT
  host: developer.dhl.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 20 03:04:41 2027 GMT
  host: api.dhl.com
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Dhl Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for DHL, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: DHL
provider_slug: dhl
slug: dhl-domain-security
source_filename: dhl-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developer.dhl.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 31 04:01:35 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.dhl.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jan 20 03:04:41 2027 GMT\n  hsts: null\ndomains:\n- domain: dhl.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dhl/refs/heads/main/security/dhl-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Freight
- Logistics
- Shipping
- eCommerce
- Tracking
---
