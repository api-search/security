---
api_specs:
- filename: ocolo-io-guidance-api-openapi.yml
  format: yaml
  label: OCOLO Guidance API
  slug: ocolo-io-guidance-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ocolo-io/openapi/ocolo-io-guidance-api-openapi.yml
- filename: ocolo-io-openapi-json-api-openapi.yml
  format: yaml
  label: OCOLO Openapi.json API
  slug: ocolo-io-openapi-json-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ocolo-io/openapi/ocolo-io-openapi-json-api-openapi.yml
- filename: ocolo-io-project-requests-api-openapi.yml
  format: yaml
  label: OCOLO Project Requests API
  slug: ocolo-io-project-requests-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ocolo-io/openapi/ocolo-io-project-requests-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: ocolo.io
  spf: true
hosts:
- cert_expires: Feb 23 07:34:56 2027 GMT
  host: ocolo.io
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: OCOLO Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for OCOLO, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: OCOLO
provider_slug: ocolo-io
slug: ocolo-io-domain-security
source_filename: ocolo-io-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ocolo.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 23 07:34:56 2027 GMT\n  hsts: null\ndomains:\n- domain: ocolo.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/ocolo-io/security/ocolo-io-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Colocation
- Data Center Marketplace
- Enterprise IT
- Wholesale Capacity Data
- Ordering Portal Licensing
- Bid Management
---
