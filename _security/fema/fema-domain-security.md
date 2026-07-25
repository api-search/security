---
api_specs:
- filename: fema-catalog-api-openapi.yml
  format: yaml
  label: OpenFEMA Catalog API
  slug: fema-catalog-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fema/refs/heads/main/openapi/fema-catalog-api-openapi.yml
- filename: fema-disaster-declarations-api-openapi.yml
  format: yaml
  label: OpenFEMA Disaster Declarations API
  slug: fema-disaster-declarations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fema/refs/heads/main/openapi/fema-disaster-declarations-api-openapi.yml
- filename: fema-hazard-mitigation-api-openapi.yml
  format: yaml
  label: OpenFEMA Hazard Mitigation API
  slug: fema-hazard-mitigation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fema/refs/heads/main/openapi/fema-hazard-mitigation-api-openapi.yml
- filename: fema-ipaws-api-openapi.yml
  format: yaml
  label: OpenFEMA IPAWS API
  slug: fema-ipaws-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fema/refs/heads/main/openapi/fema-ipaws-api-openapi.yml
- filename: fema-nfip-api-openapi.yml
  format: yaml
  label: OpenFEMA NFIP API
  slug: fema-nfip-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fema/refs/heads/main/openapi/fema-nfip-api-openapi.yml
- filename: fema-public-assistance-api-openapi.yml
  format: yaml
  label: OpenFEMA Public Assistance API
  slug: fema-public-assistance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fema/refs/heads/main/openapi/fema-public-assistance-api-openapi.yml
- filename: fema-web-disaster-summaries-api-openapi.yml
  format: yaml
  label: OpenFEMA Web Disaster Summaries API
  slug: fema-web-disaster-summaries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fema/refs/heads/main/openapi/fema-web-disaster-summaries-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: fema.gov
  spf: true
hosts:
- cert_expires: Oct 23 23:59:59 2026 GMT
  host: www.fema.gov
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Fema Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for OpenFEMA, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: OpenFEMA
provider_slug: fema
slug: fema-domain-security
source_filename: fema-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.fema.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 23 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: fema.gov\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fema/refs/heads/main/security/fema-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Government
- Open Data
- Emergency Management
- Disaster
- FEMA
- Public Safety
---
