---
api_specs:
- filename: tradeverifyd-documents-api-openapi.yml
  format: yaml
  label: Tradeverifyd Documents API
  slug: tradeverifyd-documents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tradeverifyd/refs/heads/main/openapi/tradeverifyd-documents-api-openapi.yml
- filename: tradeverifyd-entity-api-openapi.yml
  format: yaml
  label: Tradeverifyd Entity API
  slug: tradeverifyd-entity-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tradeverifyd/refs/heads/main/openapi/tradeverifyd-entity-api-openapi.yml
- filename: tradeverifyd-flags-api-openapi.yml
  format: yaml
  label: Tradeverifyd Flags API
  slug: tradeverifyd-flags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tradeverifyd/refs/heads/main/openapi/tradeverifyd-flags-api-openapi.yml
- filename: tradeverifyd-organizations-api-openapi.yml
  format: yaml
  label: Tradeverifyd Organizations API
  slug: tradeverifyd-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tradeverifyd/refs/heads/main/openapi/tradeverifyd-organizations-api-openapi.yml
- filename: tradeverifyd-relationships-api-openapi.yml
  format: yaml
  label: Tradeverifyd Relationships API
  slug: tradeverifyd-relationships-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tradeverifyd/refs/heads/main/openapi/tradeverifyd-relationships-api-openapi.yml
- filename: tradeverifyd-reports-api-openapi.yml
  format: yaml
  label: Tradeverifyd Reports API
  slug: tradeverifyd-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tradeverifyd/refs/heads/main/openapi/tradeverifyd-reports-api-openapi.yml
- filename: tradeverifyd-risk-events-api-openapi.yml
  format: yaml
  label: Tradeverifyd Risk Events API
  slug: tradeverifyd-risk-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tradeverifyd/refs/heads/main/openapi/tradeverifyd-risk-events-api-openapi.yml
- filename: tradeverifyd-scitt-reference-apis-api-openapi.yml
  format: yaml
  label: Tradeverifyd SCITT Reference APIs API
  slug: tradeverifyd-scitt-reference-apis-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tradeverifyd/refs/heads/main/openapi/tradeverifyd-scitt-reference-apis-api-openapi.yml
- filename: tradeverifyd-shipments-api-openapi.yml
  format: yaml
  label: Tradeverifyd Shipments API
  slug: tradeverifyd-shipments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tradeverifyd/refs/heads/main/openapi/tradeverifyd-shipments-api-openapi.yml
- filename: tradeverifyd-system-api-openapi.yml
  format: yaml
  label: Tradeverifyd System API
  slug: tradeverifyd-system-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tradeverifyd/refs/heads/main/openapi/tradeverifyd-system-api-openapi.yml
- filename: tradeverifyd-transparency-log-api-openapi.yml
  format: yaml
  label: Tradeverifyd Transparency Log API
  slug: tradeverifyd-transparency-log-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tradeverifyd/refs/heads/main/openapi/tradeverifyd-transparency-log-api-openapi.yml
- filename: tradeverifyd-us-customs-api-openapi.yml
  format: yaml
  label: Tradeverifyd US Customs API
  slug: tradeverifyd-us-customs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tradeverifyd/refs/heads/main/openapi/tradeverifyd-us-customs-api-openapi.yml
- filename: tradeverifyd-verifiable-credentials-api-openapi.yml
  format: yaml
  label: Tradeverifyd Verifiable Credentials API
  slug: tradeverifyd-verifiable-credentials-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tradeverifyd/refs/heads/main/openapi/tradeverifyd-verifiable-credentials-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: tradeverifyd.com
  spf: true
hosts:
- cert_expires: Oct 18 13:51:14 2026 GMT
  host: tradeverifyd.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 11 03:03:04 2026 GMT
  host: api.tradeverifyd.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Tradeverifyd Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Tradeverifyd, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Tradeverifyd
provider_slug: tradeverifyd
slug: tradeverifyd-domain-security
source_filename: tradeverifyd-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: tradeverifyd.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 18 13:51:14 2026 GMT\n  hsts: false\n- host: api.tradeverifyd.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 11 03:03:04 2026 GMT\n  hsts: null\ndomains:\n- domain: tradeverifyd.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tradeverifyd/refs/heads/main/security/tradeverifyd-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Supply Chain
- Trade Compliance
- Risk Management
- Verifiable Credentials
- Customs
- Entity Resolution
- Logistics
---
