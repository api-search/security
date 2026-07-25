---
api_specs:
- filename: packlink-clients-api-openapi.yml
  format: yaml
  label: Packlink Clients API
  slug: packlink-clients-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/packlink/refs/heads/main/openapi/packlink-clients-api-openapi.yml
- filename: packlink-customs-api-openapi.yml
  format: yaml
  label: Packlink Customs API
  slug: packlink-customs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/packlink/refs/heads/main/openapi/packlink-customs-api-openapi.yml
- filename: packlink-integrations-api-openapi.yml
  format: yaml
  label: Packlink Integrations API
  slug: packlink-integrations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/packlink/refs/heads/main/openapi/packlink-integrations-api-openapi.yml
- filename: packlink-locations-api-openapi.yml
  format: yaml
  label: Packlink Locations API
  slug: packlink-locations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/packlink/refs/heads/main/openapi/packlink-locations-api-openapi.yml
- filename: packlink-services-api-openapi.yml
  format: yaml
  label: Packlink Services API
  slug: packlink-services-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/packlink/refs/heads/main/openapi/packlink-services-api-openapi.yml
- filename: packlink-shipments-api-openapi.yml
  format: yaml
  label: Packlink Shipments API
  slug: packlink-shipments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/packlink/refs/heads/main/openapi/packlink-shipments-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: packlink.com
  spf: true
hosts:
- cert_expires: Oct 12 20:06:55 2026 GMT
  host: www.packlink.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Packlink Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Packlink, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Packlink
provider_slug: packlink
slug: packlink-domain-security
source_filename: packlink-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.packlink.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 12 20:06:55 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: packlink.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/packlink/refs/heads/main/security/packlink-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Ecommerce
- Shipping
- Logistics
- Parcel Delivery
- Carriers
- Fulfillment
---
