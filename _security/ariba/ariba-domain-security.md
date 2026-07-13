---
api_specs:
- filename: openapi.json
  format: json
  label: Ariba Network API
  slug: ariba-network-api
  spec_type: OpenAPI
  url: https://developer.ariba.com/api/network/openapi.json
- filename: openapi.json
  format: json
  label: Ariba Procurement API
  slug: ariba-procurement-api
  spec_type: OpenAPI
  url: https://developer.ariba.com/api/procurement/openapi.json
- filename: openapi.json
  format: json
  label: Ariba Sourcing API
  slug: ariba-sourcing-api
  spec_type: OpenAPI
  url: https://developer.ariba.com/api/sourcing/openapi.json
- filename: openapi.json
  format: json
  label: Ariba Contracts API
  slug: ariba-contracts-api
  spec_type: OpenAPI
  url: https://developer.ariba.com/api/contracts/openapi.json
- filename: openapi.json
  format: json
  label: Ariba Supplier API
  slug: ariba-supplier-api
  spec_type: OpenAPI
  url: https://developer.ariba.com/api/supplier/openapi.json
- filename: openapi.json
  format: json
  label: Ariba Analytics API
  slug: ariba-analytics-api
  spec_type: OpenAPI
  url: https://developer.ariba.com/api/analytics/openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: ariba.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: sap.com
  spf: true
hosts:
- cert_expires: Mar 22 23:59:59 2027 GMT
  host: developer.ariba.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 11 23:59:59 2026 GMT
  host: api.ariba.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 25 23:59:59 2026 GMT
  host: help.sap.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Ariba Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Ariba, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Ariba
provider_slug: ariba
slug: ariba-domain-security
source_filename: ariba-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developer.ariba.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 22 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 15552000\n- host: api.ariba.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 11 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: help.sap.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 25 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: ariba.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: sap.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ariba/refs/heads/main/security/ariba-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- B2B
- Catalog Management
- Compliance
- Contracts
- Enterprise
- Integration
- Invoicing
- Procurement
- Risk Management
- SAP
- Sourcing
- Spend Analysis
- Supplier Lifecycle
- Suppliers
- Supply Chain
---
