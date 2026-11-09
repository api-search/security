---
api_specs:
- filename: carrierscrub-com-authority-history-api-openapi.yml
  format: yaml
  label: CarrierScrub Authority History API
  slug: carrierscrub-com-authority-history-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/carrierscrub-com/openapi/carrierscrub-com-authority-history-api-openapi.yml
- filename: carrierscrub-com-batch-api-openapi.yml
  format: yaml
  label: CarrierScrub Batch API
  slug: carrierscrub-com-batch-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/carrierscrub-com/openapi/carrierscrub-com-batch-api-openapi.yml
- filename: carrierscrub-com-fmcsa-activity-api-openapi.yml
  format: yaml
  label: CarrierScrub Fmcsa Activity API
  slug: carrierscrub-com-fmcsa-activity-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/carrierscrub-com/openapi/carrierscrub-com-fmcsa-activity-api-openapi.yml
- filename: carrierscrub-com-lookup-api-openapi.yml
  format: yaml
  label: CarrierScrub Lookup API
  slug: carrierscrub-com-lookup-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/carrierscrub-com/openapi/carrierscrub-com-lookup-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: carrierscrub.com
  spf: true
hosts:
- cert_expires: Dec  6 21:35:11 2026 GMT
  host: carrierscrub.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Carrierscrub Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for CarrierScrub, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: CarrierScrub
provider_slug: carrierscrub-com
slug: carrierscrub-com-domain-security
source_filename: carrierscrub-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-03'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: carrierscrub.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  6 21:35:11 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: carrierscrub.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/carrierscrub-com/security/carrierscrub-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- carrier-vetting
- Freight Brokerage
- FMCSA Data
---
