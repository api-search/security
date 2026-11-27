---
api_specs:
- filename: skr-se-dataset-api-openapi.yml
  format: yaml
  label: Sveriges Kommuner och Regioner Dataset API
  slug: skr-se-dataset-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/skr-se/openapi/skr-se-dataset-api-openapi.yml
- filename: skr-se-datasets-api-openapi.yml
  format: yaml
  label: Sveriges Kommuner och Regioner Datasets API
  slug: skr-se-datasets-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/skr-se/openapi/skr-se-datasets-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: skr.se
  spf: true
hosts:
- cert_expires: Dec 23 03:06:22 2026 GMT
  host: skr.se
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Sveriges Kommuner och Regioner Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Sveriges Kommuner och Regioner, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Sveriges Kommuner och Regioner
provider_slug: skr-se
slug: skr-se-domain-security
source_filename: skr-se-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-10'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: skr.se\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 23 03:06:22 2026 GMT\n  hsts: false\ndomains:\n- domain: skr.se\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/skr-se/security/skr-se-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
- Government
- Local Government
- Open Data
- Sweden
- Public Sector
- Statistics
- Healthcare
---
