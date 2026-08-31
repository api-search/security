---
api_specs:
- filename: eia-aeo-api-openapi.yml
  format: yaml
  label: EIA AEO API
  slug: eia-aeo-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/eia/refs/heads/main/openapi/eia-aeo-api-openapi.yml
- filename: eia-coal-api-openapi.yml
  format: yaml
  label: EIA COAL API
  slug: eia-coal-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/eia/refs/heads/main/openapi/eia-coal-api-openapi.yml
- filename: eia-crud-imports-api-openapi.yml
  format: yaml
  label: EIA CRUD IMPORTS API
  slug: eia-crud-imports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/eia/refs/heads/main/openapi/eia-crud-imports-api-openapi.yml
- filename: eia-dbf-api-openapi.yml
  format: yaml
  label: EIA DBF API
  slug: eia-dbf-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/eia/refs/heads/main/openapi/eia-dbf-api-openapi.yml
- filename: eia-elec-api-openapi.yml
  format: yaml
  label: EIA ELEC API
  slug: eia-elec-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/eia/refs/heads/main/openapi/eia-elec-api-openapi.yml
- filename: eia-emiss-api-openapi.yml
  format: yaml
  label: EIA EMISS API
  slug: eia-emiss-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/eia/refs/heads/main/openapi/eia-emiss-api-openapi.yml
- filename: eia-ieo-api-openapi.yml
  format: yaml
  label: EIA IEO API
  slug: eia-ieo-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/eia/refs/heads/main/openapi/eia-ieo-api-openapi.yml
- filename: eia-intl-api-openapi.yml
  format: yaml
  label: EIA INTL API
  slug: eia-intl-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/eia/refs/heads/main/openapi/eia-intl-api-openapi.yml
- filename: eia-ng-api-openapi.yml
  format: yaml
  label: EIA NG API
  slug: eia-ng-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/eia/refs/heads/main/openapi/eia-ng-api-openapi.yml
- filename: eia-nuc-status-api-openapi.yml
  format: yaml
  label: EIA NUC STATUS API
  slug: eia-nuc-status-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/eia/refs/heads/main/openapi/eia-nuc-status-api-openapi.yml
- filename: eia-root-api-openapi.yml
  format: yaml
  label: EIA Root API
  slug: eia-root-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/eia/refs/heads/main/openapi/eia-root-api-openapi.yml
- filename: eia-rto-api-openapi.yml
  format: yaml
  label: EIA RTO API
  slug: eia-rto-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/eia/refs/heads/main/openapi/eia-rto-api-openapi.yml
- filename: eia-seds-api-openapi.yml
  format: yaml
  label: EIA SEDS API
  slug: eia-seds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/eia/refs/heads/main/openapi/eia-seds-api-openapi.yml
- filename: eia-sep-api-openapi.yml
  format: yaml
  label: EIA SEP API
  slug: eia-sep-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/eia/refs/heads/main/openapi/eia-sep-api-openapi.yml
- filename: eia-steo-api-openapi.yml
  format: yaml
  label: EIA STEO API
  slug: eia-steo-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/eia/refs/heads/main/openapi/eia-steo-api-openapi.yml
- filename: eia-total-api-openapi.yml
  format: yaml
  label: EIA TOTAL API
  slug: eia-total-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/eia/refs/heads/main/openapi/eia-total-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: eia.gov
  spf: true
hosts:
- cert_expires: Aug 19 23:59:59 2026 GMT
  host: www.eia.gov
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 18 17:20:52 2026 GMT
  host: api.eia.gov
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Eia Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for EIA, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: EIA
provider_slug: eia
slug: eia-domain-security
source_filename: eia-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-27'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.eia.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 19 23:59:59 2026 GMT\n  hsts: null\n- host: api.eia.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 18 17:20:52 2026 GMT\n  hsts: null\ndomains:\n- domain: eia.gov\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/eia/refs/heads/main/security/eia-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Energy
- United States
- Energy Markets
- Electricity
- Natural Gas
- Petroleum
- Coal
- Nuclear
- Renewables
- Grid
- Emissions
- Government
- Open Data
- Energy Statistics
---
