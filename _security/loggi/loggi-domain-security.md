---
api_specs:
- filename: loggi-authapi-api-openapi.yml
  format: yaml
  label: Loggi Auth API
  slug: loggi-authapi-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/loggi/refs/heads/main/openapi/loggi-authapi-api-openapi.yml
- filename: loggi-detailsapi-api-openapi.yml
  format: yaml
  label: Loggi Details API
  slug: loggi-detailsapi-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/loggi/refs/heads/main/openapi/loggi-detailsapi-api-openapi.yml
- filename: loggi-dropofflocationsapi-api-openapi.yml
  format: yaml
  label: Loggi Dropoff Locations API
  slug: loggi-dropofflocationsapi-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/loggi/refs/heads/main/openapi/loggi-dropofflocationsapi-api-openapi.yml
- filename: loggi-integratorcompanyapi-api-openapi.yml
  format: yaml
  label: Loggi Integrator Company API
  slug: loggi-integratorcompanyapi-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/loggi/refs/heads/main/openapi/loggi-integratorcompanyapi-api-openapi.yml
- filename: loggi-labelapi-api-openapi.yml
  format: yaml
  label: Loggi Label API
  slug: loggi-labelapi-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/loggi/refs/heads/main/openapi/loggi-labelapi-api-openapi.yml
- filename: loggi-packagecancelapi-api-openapi.yml
  format: yaml
  label: Loggi Package Cancel API
  slug: loggi-packagecancelapi-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/loggi/refs/heads/main/openapi/loggi-packagecancelapi-api-openapi.yml
- filename: loggi-packageupdateapi-api-openapi.yml
  format: yaml
  label: Loggi Package Update API
  slug: loggi-packageupdateapi-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/loggi/refs/heads/main/openapi/loggi-packageupdateapi-api-openapi.yml
- filename: loggi-quotationapi-api-openapi.yml
  format: yaml
  label: Loggi Quotation API
  slug: loggi-quotationapi-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/loggi/refs/heads/main/openapi/loggi-quotationapi-api-openapi.yml
- filename: loggi-shipmentapi-api-openapi.yml
  format: yaml
  label: Loggi Shipment API
  slug: loggi-shipmentapi-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/loggi/refs/heads/main/openapi/loggi-shipmentapi-api-openapi.yml
- filename: loggi-trackingapi-api-openapi.yml
  format: yaml
  label: Loggi Tracking API
  slug: loggi-trackingapi-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/loggi/refs/heads/main/openapi/loggi-trackingapi-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: loggi.com
  spf: true
hosts:
- cert_expires: Sep 16 12:44:39 2026 GMT
  host: www.loggi.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Loggi Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Loggi, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Loggi
provider_slug: loggi
slug: loggi-domain-security
source_filename: loggi-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.loggi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 16 12:44:39 2026 GMT\n  hsts: false\ndomains:\n- domain: loggi.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/loggi/refs/heads/main/security/loggi-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Logistics
- Shipping
- Last Mile Delivery
- Freight
- Tracking
- Brazil
---
