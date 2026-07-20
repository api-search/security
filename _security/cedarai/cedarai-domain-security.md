---
api_specs:
- filename: cedarai-external-openapi.yml
  format: yaml
  label: Cedar ARMS External API
  slug: cedar-arms-external-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cedarai/refs/heads/main/openapi/cedarai-external-openapi.yml
- filename: cedarai-work-order-openapi.yml
  format: yaml
  label: Cedar ARMS Work Order API
  slug: cedar-arms-work-order-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cedarai/refs/heads/main/openapi/cedarai-work-order-openapi.yml
- filename: cedarai-charge-openapi.yml
  format: yaml
  label: Cedar ARMS Charges API
  slug: cedar-arms-charges-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cedarai/refs/heads/main/openapi/cedarai-charge-openapi.yml
- filename: cedarai-invoices-openapi.yml
  format: yaml
  label: Cedar ARMS Shipper Invoices API
  slug: cedar-arms-shipper-invoices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cedarai/refs/heads/main/openapi/cedarai-invoices-openapi.yml
- filename: cedarai-quotes-openapi.yml
  format: yaml
  label: Cedar ARMS Shipper Quotes API
  slug: cedar-arms-shipper-quotes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cedarai/refs/heads/main/openapi/cedarai-quotes-openapi.yml
- filename: cedarai-load-tender-openapi.yml
  format: yaml
  label: Cedar ARMS Truck Load Tender API
  slug: cedar-arms-truck-load-tender-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cedarai/refs/heads/main/openapi/cedarai-load-tender-openapi.yml
- filename: cedarai-network-structure-openapi.yml
  format: yaml
  label: Cedar ARMS Network Structure API
  slug: cedar-arms-network-structure-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cedarai/refs/heads/main/openapi/cedarai-network-structure-openapi.yml
- filename: cedarai-linda-notes-openapi.yml
  format: yaml
  label: Cedar Linda Notes API
  slug: cedar-linda-notes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cedarai/refs/heads/main/openapi/cedarai-linda-notes-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: cedarai.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: cedarai.se
  spf: false
hosts:
- cert_expires: Oct 23 23:59:59 2026 GMT
  host: cedarai.com
  hsts: false
  https: true
  tls_version: TLSv1.2
- cert_expires: Nov 26 23:59:59 2026 GMT
  host: api-lg-k-h1.arms.cedarai.com
  hsts: null
  https: true
  tls_version: TLSv1.2
- host: api-lg-k-h1.arms.cedarai.se
  https: false
kind: domain-security
layout: security
method: probed
name: Cedarai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cedarai, probed live across 3 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Cedarai
provider_slug: cedarai
slug: cedarai-domain-security
source_filename: cedarai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: cedarai.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct 23 23:59:59 2026 GMT\n  hsts: false\n- host: api-lg-k-h1.arms.cedarai.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Nov 26 23:59:59 2026 GMT\n  hsts: null\n- host: api-lg-k-h1.arms.cedarai.se\n  https: false\ndomains:\n- domain: cedarai.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: cedarai.se\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cedarai/refs/heads/main/security/cedarai-domain-security.yml
summary_line: TLSv1.2 · DMARC
tags:
- Company
- Rail
- Transportation
- Logistics
- Freight
- Supply Chain
- Railcar Management
- Transportation Management System
- Fleet Management
- Artificial Intelligence
---
