---
api_specs:
- filename: fabtally-com-attest-api-openapi.yml
  format: yaml
  label: fabtally-com Attest API
  slug: fabtally-com-attest-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fabtally-com/openapi/fabtally-com-attest-api-openapi.yml
- filename: fabtally-com-dfm-api-openapi.yml
  format: yaml
  label: fabtally-com DFM API
  slug: fabtally-com-dfm-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fabtally-com/openapi/fabtally-com-dfm-api-openapi.yml
- filename: fabtally-com-discovery-api-openapi.yml
  format: yaml
  label: fabtally-com Discovery API
  slug: fabtally-com-discovery-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fabtally-com/openapi/fabtally-com-discovery-api-openapi.yml
- filename: fabtally-com-quote-api-openapi.yml
  format: yaml
  label: fabtally-com Quote API
  slug: fabtally-com-quote-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fabtally-com/openapi/fabtally-com-quote-api-openapi.yml
- filename: fabtally-com-slice-api-openapi.yml
  format: yaml
  label: fabtally-com Slice API
  slug: fabtally-com-slice-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fabtally-com/openapi/fabtally-com-slice-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: fabtally.com
  spf: true
hosts:
- cert_expires: Dec 27 20:14:09 2026 GMT
  host: fabtally.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Fabtally Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for fabtally-com, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: fabtally-com
provider_slug: fabtally-com
slug: fabtally-com-domain-security
source_filename: fabtally-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: fabtally.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 27 20:14:09 2026 GMT\n  hsts: false\ndomains:\n- domain: fabtally.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/fabtally-com/security/fabtally-com-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- 3D-printing
- Slicing
- Quotes
- API
- Manufacturing
---
