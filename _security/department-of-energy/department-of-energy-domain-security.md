---
api_specs:
- filename: department-of-energy-aeo-api-openapi.yml
  format: yaml
  label: Department of Energy Aeo API
  slug: department-of-energy-aeo-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/department-of-energy/refs/heads/main/openapi/department-of-energy-aeo-api-openapi.yml
- filename: department-of-energy-co2-emissions-api-openapi.yml
  format: yaml
  label: Department of Energy Co2 Emissions API
  slug: department-of-energy-co2-emissions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/department-of-energy/refs/heads/main/openapi/department-of-energy-co2-emissions-api-openapi.yml
- filename: department-of-energy-coal-api-openapi.yml
  format: yaml
  label: Department of Energy Coal API
  slug: department-of-energy-coal-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/department-of-energy/refs/heads/main/openapi/department-of-energy-coal-api-openapi.yml
- filename: department-of-energy-eia-open-data-api-v2-api-openapi.yml
  format: yaml
  label: Department of Energy EIA Open Data API V2 API
  slug: department-of-energy-eia-open-data-api-v2-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/department-of-energy/refs/heads/main/openapi/department-of-energy-eia-open-data-api-v2-api-openapi.yml
- filename: department-of-energy-electricity-api-openapi.yml
  format: yaml
  label: Department of Energy Electricity API
  slug: department-of-energy-electricity-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/department-of-energy/refs/heads/main/openapi/department-of-energy-electricity-api-openapi.yml
- filename: department-of-energy-international-api-openapi.yml
  format: yaml
  label: Department of Energy International API
  slug: department-of-energy-international-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/department-of-energy/refs/heads/main/openapi/department-of-energy-international-api-openapi.yml
- filename: department-of-energy-natural-gas-api-openapi.yml
  format: yaml
  label: Department of Energy Natural Gas API
  slug: department-of-energy-natural-gas-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/department-of-energy/refs/heads/main/openapi/department-of-energy-natural-gas-api-openapi.yml
- filename: department-of-energy-nuclear-outages-api-openapi.yml
  format: yaml
  label: Department of Energy Nuclear Outages API
  slug: department-of-energy-nuclear-outages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/department-of-energy/refs/heads/main/openapi/department-of-energy-nuclear-outages-api-openapi.yml
- filename: department-of-energy-petroleum-api-openapi.yml
  format: yaml
  label: Department of Energy Petroleum API
  slug: department-of-energy-petroleum-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/department-of-energy/refs/heads/main/openapi/department-of-energy-petroleum-api-openapi.yml
- filename: department-of-energy-seds-api-openapi.yml
  format: yaml
  label: Department of Energy Seds API
  slug: department-of-energy-seds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/department-of-energy/refs/heads/main/openapi/department-of-energy-seds-api-openapi.yml
- filename: department-of-energy-seriesid-api-openapi.yml
  format: yaml
  label: Department of Energy Seriesid API
  slug: department-of-energy-seriesid-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/department-of-energy/refs/heads/main/openapi/department-of-energy-seriesid-api-openapi.yml
- filename: department-of-energy-steo-api-openapi.yml
  format: yaml
  label: Department of Energy Steo API
  slug: department-of-energy-steo-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/department-of-energy/refs/heads/main/openapi/department-of-energy-steo-api-openapi.yml
- filename: department-of-energy-total-energy-api-openapi.yml
  format: yaml
  label: Department of Energy Total Energy API
  slug: department-of-energy-total-energy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/department-of-energy/refs/heads/main/openapi/department-of-energy-total-energy-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: energy.gov
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: eia.gov
  spf: true
hosts:
- cert_expires: Sep 26 23:59:59 2026 GMT
  host: www.energy.gov
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
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
name: Department Of Energy Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Department of Energy, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Department of Energy
provider_slug: department-of-energy
slug: department-of-energy-domain-security
source_filename: department-of-energy-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.energy.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 26 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: www.eia.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 19 23:59:59 2026 GMT\n  hsts: null\n- host: api.eia.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 18 17:20:52 2026 GMT\n  hsts: null\ndomains:\n- domain: energy.gov\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: eia.gov\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/department-of-energy/refs/heads/main/security/department-of-energy-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Buildings
- Electricity
- Energy
- Federal-Government
- Open Data
- Renewables
- Research
- Solar
- Statistics
---
