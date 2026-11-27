---
api_specs:
- filename: suomi-fi-connection-api-openapi.yml
  format: yaml
  label: Suomi.fi Connection API
  slug: suomi-fi-connection-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/suomi-fi/openapi/suomi-fi-connection-api-openapi.yml
- filename: suomi-fi-countries-api-openapi.yml
  format: yaml
  label: Suomi.fi Countries API
  slug: suomi-fi-countries-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/suomi-fi/openapi/suomi-fi-countries-api-openapi.yml
- filename: suomi-fi-general-description-api-openapi.yml
  format: yaml
  label: Suomi.fi General description API
  slug: suomi-fi-general-description-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/suomi-fi/openapi/suomi-fi-general-description-api-openapi.yml
- filename: suomi-fi-health-check-api-openapi.yml
  format: yaml
  label: Suomi.fi Health check API
  slug: suomi-fi-health-check-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/suomi-fi/openapi/suomi-fi-health-check-api-openapi.yml
- filename: suomi-fi-industrial-classes-api-openapi.yml
  format: yaml
  label: Suomi.fi Industrial classes API
  slug: suomi-fi-industrial-classes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/suomi-fi/openapi/suomi-fi-industrial-classes-api-openapi.yml
- filename: suomi-fi-languages-api-openapi.yml
  format: yaml
  label: Suomi.fi Languages API
  slug: suomi-fi-languages-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/suomi-fi/openapi/suomi-fi-languages-api-openapi.yml
- filename: suomi-fi-life-events-api-openapi.yml
  format: yaml
  label: Suomi.fi Life events API
  slug: suomi-fi-life-events-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/suomi-fi/openapi/suomi-fi-life-events-api-openapi.yml
- filename: suomi-fi-municipalities-api-openapi.yml
  format: yaml
  label: Suomi.fi Municipalities API
  slug: suomi-fi-municipalities-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/suomi-fi/openapi/suomi-fi-municipalities-api-openapi.yml
- filename: suomi-fi-ontology-terms-api-openapi.yml
  format: yaml
  label: Suomi.fi Ontology terms API
  slug: suomi-fi-ontology-terms-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/suomi-fi/openapi/suomi-fi-ontology-terms-api-openapi.yml
- filename: suomi-fi-organization-api-openapi.yml
  format: yaml
  label: Suomi.fi Organization API
  slug: suomi-fi-organization-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/suomi-fi/openapi/suomi-fi-organization-api-openapi.yml
- filename: suomi-fi-postal-codes-api-openapi.yml
  format: yaml
  label: Suomi.fi Postal codes API
  slug: suomi-fi-postal-codes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/suomi-fi/openapi/suomi-fi-postal-codes-api-openapi.yml
- filename: suomi-fi-regions-api-openapi.yml
  format: yaml
  label: Suomi.fi Regions API
  slug: suomi-fi-regions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/suomi-fi/openapi/suomi-fi-regions-api-openapi.yml
- filename: suomi-fi-service-api-openapi.yml
  format: yaml
  label: Suomi.fi Service API
  slug: suomi-fi-service-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/suomi-fi/openapi/suomi-fi-service-api-openapi.yml
- filename: suomi-fi-service-channel-api-openapi.yml
  format: yaml
  label: Suomi.fi Service channel API
  slug: suomi-fi-service-channel-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/suomi-fi/openapi/suomi-fi-service-channel-api-openapi.yml
- filename: suomi-fi-service-classes-api-openapi.yml
  format: yaml
  label: Suomi.fi Service classes API
  slug: suomi-fi-service-classes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/suomi-fi/openapi/suomi-fi-service-classes-api-openapi.yml
- filename: suomi-fi-service-collection-api-openapi.yml
  format: yaml
  label: Suomi.fi Service collection API
  slug: suomi-fi-service-collection-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/suomi-fi/openapi/suomi-fi-service-collection-api-openapi.yml
- filename: suomi-fi-target-groups-api-openapi.yml
  format: yaml
  label: Suomi.fi Target groups API
  slug: suomi-fi-target-groups-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/suomi-fi/openapi/suomi-fi-target-groups-api-openapi.yml
- filename: suomi-fi-wellbeing-services-counties-api-openapi.yml
  format: yaml
  label: Suomi.fi Wellbeing services counties API
  slug: suomi-fi-wellbeing-services-counties-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/suomi-fi/openapi/suomi-fi-wellbeing-services-counties-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: suomi.fi
  spf: true
hosts:
- cert_expires: May 11 23:59:59 2027 GMT
  host: kehittajille.suomi.fi
  hsts: true
  hsts_max_age: 604800
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Suomi.fi Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Suomi.fi, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Suomi.fi
provider_slug: suomi-fi
slug: suomi-fi-domain-security
source_filename: suomi-fi-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-10'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: kehittajille.suomi.fi\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: May 11 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 604800\ndomains:\n- domain: suomi.fi\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/suomi-fi/security/suomi-fi-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Government
- Finland
- Public Sector
- Digital Identity
- Service Catalogue
- Open Data
- X-Road
---
