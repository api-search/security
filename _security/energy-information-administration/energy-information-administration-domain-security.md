---
api_specs:
- filename: energy-information-administration-co2-emissions-api-openapi.yml
  format: yaml
  label: Energy Information Administration CO2 Emissions API
  slug: energy-information-administration-co2-emissions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/energy-information-administration/refs/heads/main/openapi/energy-information-administration-co2-emissions-api-openapi.yml
- filename: energy-information-administration-coal-api-openapi.yml
  format: yaml
  label: Energy Information Administration Coal API
  slug: energy-information-administration-coal-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/energy-information-administration/refs/heads/main/openapi/energy-information-administration-coal-api-openapi.yml
- filename: energy-information-administration-discovery-api-openapi.yml
  format: yaml
  label: Energy Information Administration Discovery API
  slug: energy-information-administration-discovery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/energy-information-administration/refs/heads/main/openapi/energy-information-administration-discovery-api-openapi.yml
- filename: energy-information-administration-electricity-api-openapi.yml
  format: yaml
  label: Energy Information Administration Electricity API
  slug: energy-information-administration-electricity-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/energy-information-administration/refs/heads/main/openapi/energy-information-administration-electricity-api-openapi.yml
- filename: energy-information-administration-international-api-openapi.yml
  format: yaml
  label: Energy Information Administration International API
  slug: energy-information-administration-international-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/energy-information-administration/refs/heads/main/openapi/energy-information-administration-international-api-openapi.yml
- filename: energy-information-administration-natural-gas-api-openapi.yml
  format: yaml
  label: Energy Information Administration Natural Gas API
  slug: energy-information-administration-natural-gas-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/energy-information-administration/refs/heads/main/openapi/energy-information-administration-natural-gas-api-openapi.yml
- filename: energy-information-administration-nuclear-api-openapi.yml
  format: yaml
  label: Energy Information Administration Nuclear API
  slug: energy-information-administration-nuclear-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/energy-information-administration/refs/heads/main/openapi/energy-information-administration-nuclear-api-openapi.yml
- filename: energy-information-administration-petroleum-api-openapi.yml
  format: yaml
  label: Energy Information Administration Petroleum API
  slug: energy-information-administration-petroleum-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/energy-information-administration/refs/heads/main/openapi/energy-information-administration-petroleum-api-openapi.yml
- filename: energy-information-administration-seds-api-openapi.yml
  format: yaml
  label: Energy Information Administration SEDS API
  slug: energy-information-administration-seds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/energy-information-administration/refs/heads/main/openapi/energy-information-administration-seds-api-openapi.yml
- filename: energy-information-administration-total-energy-api-openapi.yml
  format: yaml
  label: Energy Information Administration Total Energy API
  slug: energy-information-administration-total-energy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/energy-information-administration/refs/heads/main/openapi/energy-information-administration-total-energy-api-openapi.yml
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
name: Energy Information Administration Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Energy Information Administration, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Energy Information Administration
provider_slug: energy-information-administration
slug: energy-information-administration-domain-security
source_filename: energy-information-administration-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.eia.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 19 23:59:59 2026 GMT\n  hsts: null\n- host: api.eia.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 18 17:20:52 2026 GMT\n  hsts: null\ndomains:\n- domain: eia.gov\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/energy-information-administration/refs/heads/main/security/energy-information-administration-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Energy
- Federal-Government
- Open Data
---
