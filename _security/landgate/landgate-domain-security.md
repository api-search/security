---
api_specs:
- filename: landgate-datasets-api-openapi.yml
  format: yaml
  label: Landgate Datasets API
  slug: landgate-datasets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/landgate/refs/heads/main/openapi/landgate-datasets-api-openapi.yml
- filename: landgate-discovery-api-openapi.yml
  format: yaml
  label: Landgate Discovery API
  slug: landgate-discovery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/landgate/refs/heads/main/openapi/landgate-discovery-api-openapi.yml
- filename: landgate-organizations-api-openapi.yml
  format: yaml
  label: Landgate Organizations API
  slug: landgate-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/landgate/refs/heads/main/openapi/landgate-organizations-api-openapi.yml
- filename: landgate-query-api-openapi.yml
  format: yaml
  label: Landgate Query API
  slug: landgate-query-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/landgate/refs/heads/main/openapi/landgate-query-api-openapi.yml
- filename: landgate-server-api-openapi.yml
  format: yaml
  label: Landgate Server API
  slug: landgate-server-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/landgate/refs/heads/main/openapi/landgate-server-api-openapi.yml
- filename: landgate-services-api-openapi.yml
  format: yaml
  label: Landgate Services API
  slug: landgate-services-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/landgate/refs/heads/main/openapi/landgate-services-api-openapi.yml
- filename: landgate-site-api-openapi.yml
  format: yaml
  label: Landgate Site API
  slug: landgate-site-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/landgate/refs/heads/main/openapi/landgate-site-api-openapi.yml
- filename: landgate-wfs-api-openapi.yml
  format: yaml
  label: Landgate WFS API
  slug: landgate-wfs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/landgate/refs/heads/main/openapi/landgate-wfs-api-openapi.yml
- filename: landgate-wms-api-openapi.yml
  format: yaml
  label: Landgate WMS API
  slug: landgate-wms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/landgate/refs/heads/main/openapi/landgate-wms-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: wa.gov.au
  spf: true
hosts:
- cert_expires: Oct  4 22:03:15 2026 GMT
  host: www.landgate.wa.gov.au
  hsts: true
  hsts_max_age: 2592000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 20 23:59:59 2026 GMT
  host: www.data.wa.gov.au
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Mar 18 23:59:59 2027 GMT
  host: public-services.slip.wa.gov.au
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Landgate Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Landgate, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Landgate
provider_slug: landgate
slug: landgate-domain-security
source_filename: landgate-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.landgate.wa.gov.au\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 22:03:15 2026 GMT\n  hsts: true\n  hsts_max_age: 2592000\n- host: www.data.wa.gov.au\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 20 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: public-services.slip.wa.gov.au\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 18 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: wa.gov.au\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/landgate/refs/heads/main/security/landgate-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Real-Estate
- Australia
- Land Registry
- Title
- Valuation
- Property Data
- Open Data
- Geospatial
- Government
- Conveyancing
- PropTech
---
