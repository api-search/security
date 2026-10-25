---
api_specs:
- filename: descartes-3rd-party-tms-integration-api-openapi.yml
  format: yaml
  label: Descartes Systems Group 3rd Party TMS Integration API
  slug: descartes-3rd-party-tms-integration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/descartes/refs/heads/main/openapi/descartes-3rd-party-tms-integration-api-openapi.yml
- filename: descartes-api-xml-api-openapi.yml
  format: yaml
  label: Descartes Systems Group API - XML API
  slug: descartes-api-xml-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/descartes/refs/heads/main/openapi/descartes-api-xml-api-openapi.yml
- filename: descartes-carrier-data-connection-and-communication-api-openapi.yml
  format: yaml
  label: Descartes Systems Group Carrier Data Connection and Communication API
  slug: descartes-carrier-data-connection-and-communication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/descartes/refs/heads/main/openapi/descartes-carrier-data-connection-and-communication-api-openapi.yml
- filename: descartes-custom-integration-api-openapi.yml
  format: yaml
  label: Descartes Systems Group Custom Integration API
  slug: descartes-custom-integration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/descartes/refs/heads/main/openapi/descartes-custom-integration-api-openapi.yml
- filename: descartes-export-api-api-openapi.yml
  format: yaml
  label: Descartes Systems Group Export API
  slug: descartes-export-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/descartes/refs/heads/main/openapi/descartes-export-api-api-openapi.yml
- filename: descartes-fraudguard-carrier-and-load-lookup-api-openapi.yml
  format: yaml
  label: Descartes Systems Group FraudGuard Carrier and Load Lookup API
  slug: descartes-fraudguard-carrier-and-load-lookup-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/descartes/refs/heads/main/openapi/descartes-fraudguard-carrier-and-load-lookup-api-openapi.yml
- filename: descartes-import-api-api-openapi.yml
  format: yaml
  label: Descartes Systems Group Import API
  slug: descartes-import-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/descartes/refs/heads/main/openapi/descartes-import-api-api-openapi.yml
- filename: descartes-load-visibility-order-creation-xml-api-openapi.yml
  format: yaml
  label: Descartes Systems Group Load Visibility Order Creation - XML API
  slug: descartes-load-visibility-order-creation-xml-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/descartes/refs/heads/main/openapi/descartes-load-visibility-order-creation-xml-api-openapi.yml
- filename: descartes-load-visibility-url-and-data-export-retrieval-api-openapi.yml
  format: yaml
  label: Descartes Systems Group Load Visibility URL and Data Export Retrieval API
  slug: descartes-load-visibility-url-and-data-export-retrieval-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/descartes/refs/heads/main/openapi/descartes-load-visibility-url-and-data-export-retrieval-api-openapi.yml
- filename: descartes-search-api-api-openapi.yml
  format: yaml
  label: Descartes Systems Group Search API
  slug: descartes-search-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/descartes/refs/heads/main/openapi/descartes-search-api-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: descartes.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: macropoint.com
  spf: true
hosts:
- cert_expires: Nov 15 23:59:59 2026 GMT
  host: www.descartes.com
  hsts: true
  hsts_max_age: 300
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 17 08:22:36 2026 GMT
  host: docs.macropoint.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb  2 23:59:59 2027 GMT
  host: macropoint-lite.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Descartes Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Descartes Systems Group, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Descartes Systems Group
provider_slug: descartes
slug: descartes-domain-security
source_filename: descartes-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.descartes.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 15 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 300\n- host: docs.macropoint.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 17 08:22:36 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: macropoint-lite.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  2 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: descartes.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: macropoint.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/descartes/refs/heads/main/security/descartes-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Logistics
- Supply Chain
- Freight Visibility
- Shipment Tracking
- Customs Compliance
- Global Trade
- Trade Content
- Carrier Sourcing
---
