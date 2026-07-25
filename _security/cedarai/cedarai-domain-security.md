---
api_specs:
- filename: cedarai-chargeservice-api-openapi.yml
  format: yaml
  label: Cedarai ChargeService API
  slug: cedarai-chargeservice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cedarai/refs/heads/main/openapi/cedarai-chargeservice-api-openapi.yml
- filename: cedarai-equipment-history-api-openapi.yml
  format: yaml
  label: Cedarai Equipment History API
  slug: cedarai-equipment-history-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cedarai/refs/heads/main/openapi/cedarai-equipment-history-api-openapi.yml
- filename: cedarai-ims-api-openapi.yml
  format: yaml
  label: Cedarai Ims API
  slug: cedarai-ims-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cedarai/refs/heads/main/openapi/cedarai-ims-api-openapi.yml
- filename: cedarai-invoicesservice-api-openapi.yml
  format: yaml
  label: Cedarai InvoicesService API
  slug: cedarai-invoicesservice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cedarai/refs/heads/main/openapi/cedarai-invoicesservice-api-openapi.yml
- filename: cedarai-lindaservice-api-openapi.yml
  format: yaml
  label: Cedarai LindaService API
  slug: cedarai-lindaservice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cedarai/refs/heads/main/openapi/cedarai-lindaservice-api-openapi.yml
- filename: cedarai-networkstructureservice-api-openapi.yml
  format: yaml
  label: Cedarai NetworkStructureService API
  slug: cedarai-networkstructureservice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cedarai/refs/heads/main/openapi/cedarai-networkstructureservice-api-openapi.yml
- filename: cedarai-quotesservice-api-openapi.yml
  format: yaml
  label: Cedarai QuotesService API
  slug: cedarai-quotesservice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cedarai/refs/heads/main/openapi/cedarai-quotesservice-api-openapi.yml
- filename: cedarai-truckloadtenderservice-api-openapi.yml
  format: yaml
  label: Cedarai TruckLoadTenderService API
  slug: cedarai-truckloadtenderservice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cedarai/refs/heads/main/openapi/cedarai-truckloadtenderservice-api-openapi.yml
- filename: cedarai-workorderservice-api-openapi.yml
  format: yaml
  label: Cedarai WorkOrderService API
  slug: cedarai-workorderservice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cedarai/refs/heads/main/openapi/cedarai-workorderservice-api-openapi.yml
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
