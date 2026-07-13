---
api_specs:
- filename: apispec
  format: yaml
  label: USDA FoodData Central API
  slug: fooddata-central-api
  spec_type: OpenAPI
  url: https://fdc.nal.usda.gov/portal-data/external/apispec
- filename: usda-ars-ag-data-commons-openapi.yml
  format: yaml
  label: USDA Ag Data Commons CKAN API
  slug: ag-data-commons-ckan-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/usda-agricultural-research-service-ars-/refs/heads/main/openapi/usda-ars-ag-data-commons-openapi.yml
description: ''
domains:
- caa:
  - 0 iodef "mailto:icam_as_notify@ocio.usda.gov"
  - 0 issue "globalsign.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "digicert.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: usda.gov
  spf: true
hosts:
- cert_expires: Aug 10 23:59:59 2026 GMT
  host: fdc.nal.usda.gov
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
- cert_expires: Nov 26 23:59:59 2026 GMT
  host: agdatacommons.nal.usda.gov
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 10 23:59:59 2026 GMT
  host: data.nal.usda.gov
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Usda Agricultural Research Service Ars  Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for USDA Agricultural Research Service (ARS), probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.2); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: USDA Agricultural Research Service (ARS)
provider_slug: usda-agricultural-research-service-ars-
slug: usda-agricultural-research-service-ars--domain-security
source_filename: usda-agricultural-research-service-ars--domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: fdc.nal.usda.gov\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Aug 10 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: agdatacommons.nal.usda.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 26 23:59:59 2026 GMT\n  hsts: false\n- host: data.nal.usda.gov\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Aug 10 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: usda.gov\n  dnssec: true\n  caa:\n  - 0 iodef \"mailto:icam_as_notify@ocio.usda.gov\"\n  - 0 issue \"globalsign.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"digicert.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/usda-agricultural-research-service-ars-/refs/heads/main/security/usda-agricultural-research-service-ars--domain-security.yml
summary_line: TLSv1.2 · HSTS · DNSSEC · DMARC
tags:
- Federal Government
- Agriculture
- Food Safety
- Nutrition
- Open Data
- Research
---
