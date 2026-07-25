---
api_specs:
- filename: doe-aeo-api-openapi.yml
  format: yaml
  label: Department of Energy AEO API
  slug: doe-aeo-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/doe/refs/heads/main/openapi/doe-aeo-api-openapi.yml
- filename: doe-coal-api-openapi.yml
  format: yaml
  label: Department of Energy COAL API
  slug: doe-coal-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/doe/refs/heads/main/openapi/doe-coal-api-openapi.yml
- filename: doe-crud-imports-api-openapi.yml
  format: yaml
  label: Department of Energy CRUD_IMPORTS API
  slug: doe-crud-imports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/doe/refs/heads/main/openapi/doe-crud-imports-api-openapi.yml
- filename: doe-dbf-api-openapi.yml
  format: yaml
  label: Department of Energy DBF API
  slug: doe-dbf-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/doe/refs/heads/main/openapi/doe-dbf-api-openapi.yml
- filename: doe-elec-api-openapi.yml
  format: yaml
  label: Department of Energy ELEC API
  slug: doe-elec-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/doe/refs/heads/main/openapi/doe-elec-api-openapi.yml
- filename: doe-emiss-api-openapi.yml
  format: yaml
  label: Department of Energy EMISS API
  slug: doe-emiss-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/doe/refs/heads/main/openapi/doe-emiss-api-openapi.yml
- filename: doe-ieo-api-openapi.yml
  format: yaml
  label: Department of Energy IEO API
  slug: doe-ieo-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/doe/refs/heads/main/openapi/doe-ieo-api-openapi.yml
- filename: doe-intl-api-openapi.yml
  format: yaml
  label: Department of Energy INTL API
  slug: doe-intl-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/doe/refs/heads/main/openapi/doe-intl-api-openapi.yml
- filename: doe-ng-api-openapi.yml
  format: yaml
  label: Department of Energy NG API
  slug: doe-ng-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/doe/refs/heads/main/openapi/doe-ng-api-openapi.yml
- filename: doe-nuc-status-api-openapi.yml
  format: yaml
  label: Department of Energy NUC_STATUS API
  slug: doe-nuc-status-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/doe/refs/heads/main/openapi/doe-nuc-status-api-openapi.yml
- filename: doe-root-api-openapi.yml
  format: yaml
  label: Department of Energy Root API
  slug: doe-root-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/doe/refs/heads/main/openapi/doe-root-api-openapi.yml
- filename: doe-rto-api-openapi.yml
  format: yaml
  label: Department of Energy RTO API
  slug: doe-rto-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/doe/refs/heads/main/openapi/doe-rto-api-openapi.yml
- filename: doe-seds-api-openapi.yml
  format: yaml
  label: Department of Energy SEDS API
  slug: doe-seds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/doe/refs/heads/main/openapi/doe-seds-api-openapi.yml
- filename: doe-sep-api-openapi.yml
  format: yaml
  label: Department of Energy SEP API
  slug: doe-sep-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/doe/refs/heads/main/openapi/doe-sep-api-openapi.yml
- filename: doe-steo-api-openapi.yml
  format: yaml
  label: Department of Energy STEO API
  slug: doe-steo-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/doe/refs/heads/main/openapi/doe-steo-api-openapi.yml
- filename: doe-total-api-openapi.yml
  format: yaml
  label: Department of Energy TOTAL API
  slug: doe-total-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/doe/refs/heads/main/openapi/doe-total-api-openapi.yml
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
name: Doe Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Department of Energy, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Department of Energy
provider_slug: doe
slug: doe-domain-security
source_filename: doe-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.energy.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 26 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: www.eia.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 19 23:59:59 2026 GMT\n  hsts: null\n- host: api.eia.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 18 17:20:52 2026 GMT\n  hsts: null\ndomains:\n- domain: energy.gov\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: eia.gov\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/doe/refs/heads/main/security/doe-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Energy
- Government
- Renewable Energy
- Electricity
- Natural Gas
- Petroleum
- Solar
- Wind
- Electric Vehicles
- Alternative Fuels
- Nuclear
- Scientific Research
---
