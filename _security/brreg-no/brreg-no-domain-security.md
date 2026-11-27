---
api_specs:
- filename: brreg-no-enheter-api-openapi.yml
  format: yaml
  label: Brønnøysundregistrene Enheter API
  slug: brreg-no-enheter-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/brreg-no/openapi/brreg-no-enheter-api-openapi.yml
- filename: brreg-no-frivillighetsregisteret-api-openapi.yml
  format: yaml
  label: Brønnøysundregistrene Frivillighetsregisteret API
  slug: brreg-no-frivillighetsregisteret-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/brreg-no/openapi/brreg-no-frivillighetsregisteret-api-openapi.yml
- filename: brreg-no-generelt-api-openapi.yml
  format: yaml
  label: Brønnøysundregistrene Generelt API
  slug: brreg-no-generelt-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/brreg-no/openapi/brreg-no-generelt-api-openapi.yml
- filename: brreg-no-kommuner-api-openapi.yml
  format: yaml
  label: Brønnøysundregistrene Kommuner API
  slug: brreg-no-kommuner-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/brreg-no/openapi/brreg-no-kommuner-api-openapi.yml
- filename: brreg-no-kopi-av-rsregnskap-api-openapi.yml
  format: yaml
  label: Brønnøysundregistrene Kopi av årsregnskap API
  slug: brreg-no-kopi-av-rsregnskap-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/brreg-no/openapi/brreg-no-kopi-av-rsregnskap-api-openapi.yml
- filename: brreg-no-matrikkelenheter-api-openapi.yml
  format: yaml
  label: Brønnøysundregistrene Matrikkelenheter API
  slug: brreg-no-matrikkelenheter-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/brreg-no/openapi/brreg-no-matrikkelenheter-api-openapi.yml
- filename: brreg-no-mellombalanse-api-openapi.yml
  format: yaml
  label: Brønnøysundregistrene Mellombalanse API
  slug: brreg-no-mellombalanse-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/brreg-no/openapi/brreg-no-mellombalanse-api-openapi.yml
- filename: brreg-no-oppdateringer-api-openapi.yml
  format: yaml
  label: Brønnøysundregistrene Oppdateringer API
  slug: brreg-no-oppdateringer-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/brreg-no/openapi/brreg-no-oppdateringer-api-openapi.yml
- filename: brreg-no-organisasjonsformer-api-openapi.yml
  format: yaml
  label: Brønnøysundregistrene Organisasjonsformer API
  slug: brreg-no-organisasjonsformer-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/brreg-no/openapi/brreg-no-organisasjonsformer-api-openapi.yml
- filename: brreg-no-partiregisteret-api-openapi.yml
  format: yaml
  label: Brønnøysundregistrene Partiregisteret API
  slug: brreg-no-partiregisteret-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/brreg-no/openapi/brreg-no-partiregisteret-api-openapi.yml
- filename: brreg-no-regnskapsregisteret-api-openapi.yml
  format: yaml
  label: Brønnøysundregistrene Regnskapsregisteret API
  slug: brreg-no-regnskapsregisteret-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/brreg-no/openapi/brreg-no-regnskapsregisteret-api-openapi.yml
- filename: brreg-no-roller-api-openapi.yml
  format: yaml
  label: Brønnøysundregistrene Roller API
  slug: brreg-no-roller-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/brreg-no/openapi/brreg-no-roller-api-openapi.yml
- filename: brreg-no-statistikk-api-openapi.yml
  format: yaml
  label: Brønnøysundregistrene Statistikk API
  slug: brreg-no-statistikk-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/brreg-no/openapi/brreg-no-statistikk-api-openapi.yml
- filename: brreg-no-underenheter-api-openapi.yml
  format: yaml
  label: Brønnøysundregistrene Underenheter API
  slug: brreg-no-underenheter-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/brreg-no/openapi/brreg-no-underenheter-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: brreg.no
  spf: true
hosts:
- cert_expires: Jan 16 09:48:21 2027 GMT
  host: data.brreg.no
  hsts: null
  https: true
  tls_version: TLSv1.2
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Brønnøysundregistrene Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Brønnøysundregistrene, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Brønnøysundregistrene
provider_slug: brreg-no
slug: brreg-no-domain-security
source_filename: brreg-no-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-10'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: data.brreg.no\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jan 16 09:48:21 2027 GMT\n  hsts: null\ndomains:\n- domain: brreg.no\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/brreg-no/security/brreg-no-domain-security.yml
summary_line: TLSv1.2 · DNSSEC · DMARC
tags:
- Government
- Business Registry
- Open Data
- Norway
- Company Data
- Public Sector
- Financial Statements
---
