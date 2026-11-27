---
api_specs:
- filename: opencrvs-org-attachments-api-openapi.yml
  format: yaml
  label: OpenCRVS Attachments API
  slug: opencrvs-org-attachments-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/opencrvs-org/openapi/opencrvs-org-attachments-api-openapi.yml
- filename: opencrvs-org-events-api-openapi.yml
  format: yaml
  label: OpenCRVS Events API
  slug: opencrvs-org-events-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/opencrvs-org/openapi/opencrvs-org-events-api-openapi.yml
- filename: opencrvs-org-integrations-api-openapi.yml
  format: yaml
  label: OpenCRVS Integrations API
  slug: opencrvs-org-integrations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/opencrvs-org/openapi/opencrvs-org-integrations-api-openapi.yml
- filename: opencrvs-org-locations-api-openapi.yml
  format: yaml
  label: OpenCRVS Locations API
  slug: opencrvs-org-locations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/opencrvs-org/openapi/opencrvs-org-locations-api-openapi.yml
- filename: opencrvs-org-search-api-openapi.yml
  format: yaml
  label: OpenCRVS Search API
  slug: opencrvs-org-search-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/opencrvs-org/openapi/opencrvs-org-search-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: opencrvs.org
  spf: true
hosts:
- cert_expires: Jan  6 09:51:17 2027 GMT
  host: www.opencrvs.org
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: OpenCRVS Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for OpenCRVS, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: OpenCRVS
provider_slug: opencrvs-org
slug: opencrvs-org-domain-security
source_filename: opencrvs-org-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-09'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.opencrvs.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  6 09:51:17 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: opencrvs.org\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/opencrvs-org/security/opencrvs-org-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Open Source
- CivilRegistration
- Government
---
