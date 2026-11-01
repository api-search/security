---
api_specs:
- filename: algoum-de-common-api-openapi.yml
  format: yaml
  label: algoum-de Common API
  slug: algoum-de-common-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/algoum-de/openapi/algoum-de-common-api-openapi.yml
- filename: algoum-de-events-api-openapi.yml
  format: yaml
  label: algoum-de Events API
  slug: algoum-de-events-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/algoum-de/openapi/algoum-de-events-api-openapi.yml
- filename: algoum-de-insider-api-openapi.yml
  format: yaml
  label: algoum-de Insider API
  slug: algoum-de-insider-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/algoum-de/openapi/algoum-de-insider-api-openapi.yml
- filename: algoum-de-institutional-api-openapi.yml
  format: yaml
  label: algoum-de Institutional API
  slug: algoum-de-institutional-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/algoum-de/openapi/algoum-de-institutional-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: algoum.de
  spf: true
hosts:
- cert_expires: Dec 31 14:01:16 2026 GMT
  host: algoum.de
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Algoum De Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for algoum-de, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: algoum-de
provider_slug: algoum-de
slug: algoum-de-domain-security
source_filename: algoum-de-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: algoum.de\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 31 14:01:16 2026 GMT\n  hsts: false\ndomains:\n- domain: algoum.de\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/algoum-de/security/algoum-de-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Finance
- SEC
- InsiderTrading
- API
---
