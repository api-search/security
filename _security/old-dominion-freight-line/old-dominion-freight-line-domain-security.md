---
api_specs:
- filename: old-dominion-freight-line-bill-of-lading-api-openapi.yml
  format: yaml
  label: ODFL Bill of Lading API
  slug: bill-of-lading-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/old-dominion-freight-line/refs/heads/main/openapi/old-dominion-freight-line-bill-of-lading-api-openapi.yml
- filename: old-dominion-freight-line-pickup-api-openapi.yml
  format: yaml
  label: ODFL Pickup API
  slug: pickup-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/old-dominion-freight-line/refs/heads/main/openapi/old-dominion-freight-line-pickup-api-openapi.yml
- filename: old-dominion-freight-line-tracking-api-openapi.yml
  format: yaml
  label: ODFL Tracking API
  slug: tracking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/old-dominion-freight-line/refs/heads/main/openapi/old-dominion-freight-line-tracking-api-openapi.yml
- filename: old-dominion-freight-line-document-api-openapi.yml
  format: yaml
  label: ODFL Document API
  slug: document-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/old-dominion-freight-line/refs/heads/main/openapi/old-dominion-freight-line-document-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: odfl.com
  spf: true
hosts:
- cert_expires: Oct 23 23:59:59 2026 GMT
  host: www.odfl.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Old Dominion Freight Line Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Old Dominion Freight Line, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Old Dominion Freight Line
provider_slug: old-dominion-freight-line
slug: old-dominion-freight-line-domain-security
source_filename: old-dominion-freight-line-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.odfl.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 23 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: odfl.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/old-dominion-freight-line/refs/heads/main/security/old-dominion-freight-line-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Freight
- Less-Than-Truckload
- Logistics
- Shipping
- Transportation
- Fortune 1000
---
