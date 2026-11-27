---
api_specs:
- filename: hlido-eu-directory-api-openapi.yml
  format: yaml
  label: Hlido Directory API
  slug: hlido-eu-directory-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hlido-eu/openapi/hlido-eu-directory-api-openapi.yml
- filename: hlido-eu-incidents-api-openapi.yml
  format: yaml
  label: Hlido Incidents API
  slug: hlido-eu-incidents-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hlido-eu/openapi/hlido-eu-incidents-api-openapi.yml
- filename: hlido-eu-ops-api-openapi.yml
  format: yaml
  label: Hlido Ops API
  slug: hlido-eu-ops-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hlido-eu/openapi/hlido-eu-ops-api-openapi.yml
- filename: hlido-eu-recommendations-api-openapi.yml
  format: yaml
  label: Hlido Recommendations API
  slug: hlido-eu-recommendations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hlido-eu/openapi/hlido-eu-recommendations-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: hlido.eu
  spf: true
hosts:
- cert_expires: Jan  5 13:51:45 2027 GMT
  host: hlido.eu
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Hlido Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Hlido, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Hlido
provider_slug: hlido-eu
slug: hlido-eu-domain-security
source_filename: hlido-eu-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: hlido.eu\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  5 13:51:45 2027 GMT\n  hsts: false\ndomains:\n- domain: hlido.eu\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/hlido-eu/security/hlido-eu-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Satellite
- Artificial Intelligence
- Earth Observation
- Czech
- Startups
---
