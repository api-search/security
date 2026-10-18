---
api_specs:
- filename: dpd-group-countries-api-openapi.yml
  format: yaml
  label: DPD Geo Countries API
  slug: geoapi-countries
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dpd-group/refs/heads/main/openapi/dpd-group-countries-api-openapi.yml
- filename: dpd-group-customers-api-openapi.yml
  format: yaml
  label: DPD Geo Customers API
  slug: geoapi-customers
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dpd-group/refs/heads/main/openapi/dpd-group-customers-api-openapi.yml
- filename: dpd-group-me-api-openapi.yml
  format: yaml
  label: DPD Geo Me API
  slug: geoapi-me
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dpd-group/refs/heads/main/openapi/dpd-group-me-api-openapi.yml
- filename: dpd-group-parcels-api-openapi.yml
  format: yaml
  label: DPD Geo Parcels API
  slug: geoapi-parcels
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dpd-group/refs/heads/main/openapi/dpd-group-parcels-api-openapi.yml
- filename: dpd-group-pickup-orders-api-openapi.yml
  format: yaml
  label: DPD Geo Pickup Orders API
  slug: geoapi-pickup-orders
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dpd-group/refs/heads/main/openapi/dpd-group-pickup-orders-api-openapi.yml
- filename: dpd-group-shipments-api-openapi.yml
  format: yaml
  label: DPD Geo Shipments API
  slug: geoapi-shipments
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dpd-group/refs/heads/main/openapi/dpd-group-shipments-api-openapi.yml
- filename: dpd-group-shipping-services-api-openapi.yml
  format: yaml
  label: DPD Geo Shipping Services API
  slug: geoapi-shipping-services
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dpd-group/refs/heads/main/openapi/dpd-group-shipping-services-api-openapi.yml
- filename: dpd-group-shipping-api-openapi.yml
  format: yaml
  label: DPD META-API Shipment
  slug: meta-api-shipping
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dpd-group/refs/heads/main/openapi/dpd-group-shipping-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: dpd.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: dpd.cz
  spf: true
hosts:
- cert_expires: Mar 14 23:59:59 2027 GMT
  host: www.dpd.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb 23 23:59:59 2027 GMT
  host: esolutions.dpd.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb 13 23:59:59 2027 GMT
  host: geoapi.dpd.cz
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Dpd Group Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for DPD Group, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: DPD Group
provider_slug: dpd-group
slug: dpd-group-domain-security
source_filename: dpd-group-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.dpd.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 14 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: esolutions.dpd.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 23 23:59:59 2027 GMT\n  hsts: false\n- host: geoapi.dpd.cz\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 13 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: dpd.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n- domain: dpd.cz\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dpd-group/refs/heads/main/security/dpd-group-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Logistics
- Parcel
- Shipping
- Tracking
- Carrier
---
