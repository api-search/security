---
api_specs:
- filename: fema-openapi.yml
  format: yaml
  label: FEMA Disaster Declarations Summaries API
  slug: fema-disaster-declarations-summaries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fema/refs/heads/main/openapi/fema-openapi.yml
- filename: fema-openapi.yml
  format: yaml
  label: FEMA Public Assistance Funded Projects Details API
  slug: fema-public-assistance-funded-projects-details-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fema/refs/heads/main/openapi/fema-openapi.yml
- filename: fema-openapi.yml
  format: yaml
  label: FEMA Hazard Mitigation Assistance Projects API
  slug: fema-hazard-mitigation-assistance-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fema/refs/heads/main/openapi/fema-openapi.yml
- filename: fema-openapi.yml
  format: yaml
  label: FEMA NFIP Redacted Policies API
  slug: fema-nfip-redacted-policies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fema/refs/heads/main/openapi/fema-openapi.yml
- filename: fema-openapi.yml
  format: yaml
  label: FEMA NFIP Redacted Claims API
  slug: fema-nfip-redacted-claims-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fema/refs/heads/main/openapi/fema-openapi.yml
- filename: fema-openapi.yml
  format: yaml
  label: FEMA IPAWS Archived Alerts API
  slug: fema-ipaws-archived-alerts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fema/refs/heads/main/openapi/fema-openapi.yml
- filename: fema-openapi.yml
  format: yaml
  label: FEMA Web Disaster Summaries API
  slug: fema-web-disaster-summaries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fema/refs/heads/main/openapi/fema-openapi.yml
- filename: fema-openapi.yml
  format: yaml
  label: FEMA OpenFEMA Dataset Catalog API
  slug: fema-openfema-dataset-catalog-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fema/refs/heads/main/openapi/fema-openapi.yml
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
