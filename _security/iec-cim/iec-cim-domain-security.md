---
api_specs:
- filename: iec-cim-customers-api-openapi.yml
  format: yaml
  label: iec-cim Customers API
  slug: iec-cim-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/iec-cim/refs/heads/main/openapi/iec-cim-customers-api-openapi.yml
- filename: iec-cim-metering-api-openapi.yml
  format: yaml
  label: iec-cim Metering API
  slug: iec-cim-metering-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/iec-cim/refs/heads/main/openapi/iec-cim-metering-api-openapi.yml
- filename: iec-cim-network-assets-api-openapi.yml
  format: yaml
  label: iec-cim Network Assets API
  slug: iec-cim-network-assets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/iec-cim/refs/heads/main/openapi/iec-cim-network-assets-api-openapi.yml
- filename: iec-cim-outages-api-openapi.yml
  format: yaml
  label: iec-cim Outages API
  slug: iec-cim-outages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/iec-cim/refs/heads/main/openapi/iec-cim-outages-api-openapi.yml
- filename: iec-cim-work-orders-api-openapi.yml
  format: yaml
  label: iec-cim Work Orders API
  slug: iec-cim-work-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/iec-cim/refs/heads/main/openapi/iec-cim-work-orders-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: iec.ch
  spf: true
hosts:
- cert_expires: Feb 10 23:59:59 2027 GMT
  host: www.iec.ch
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Iec Cim Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for iec-cim, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: iec-cim
provider_slug: iec-cim
slug: iec-cim-domain-security
source_filename: iec-cim-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.iec.ch\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 10 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: iec.ch\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/iec-cim/refs/heads/main/security/iec-cim-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags: []
---
