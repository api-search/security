---
api_specs:
- filename: parcelsapp-openapi.yml
  format: yaml
  label: Parcels App Shipments Tracking API
  slug: parcelsapp-shipments-tracking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/parcelsapp/refs/heads/main/openapi/parcelsapp-openapi.yml
- filename: parcelsapp-openapi.yml
  format: yaml
  label: Parcels App Account Usage API
  slug: parcelsapp-account-usage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/parcelsapp/refs/heads/main/openapi/parcelsapp-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: parcelsapp.com
  spf: true
hosts:
- cert_expires: Jul 24 07:48:52 2026 GMT
  host: parcelsapp.com
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Parcelsapp Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Parcels App, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Parcels App
provider_slug: parcelsapp
slug: parcelsapp-domain-security
source_filename: parcelsapp-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: parcelsapp.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jul 24 07:48:52 2026 GMT\n  hsts: false\ndomains:\n- domain: parcelsapp.com\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/parcelsapp/refs/heads/main/security/parcelsapp-domain-security.yml
summary_line: TLSv1.2 · DMARC
tags:
- Parcel Tracking
- Shipment Status
- Package Tracking
- Logistics
- Shipping
- Carriers
---
