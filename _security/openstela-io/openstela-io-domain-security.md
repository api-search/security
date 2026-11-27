---
api_specs:
- filename: openstela-io-account-api-openapi.yml
  format: yaml
  label: OpenStela Account API
  slug: openstela-io-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/openstela-io/openapi/openstela-io-account-api-openapi.yml
- filename: openstela-io-characters-api-openapi.yml
  format: yaml
  label: OpenStela Characters API
  slug: openstela-io-characters-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/openstela-io/openapi/openstela-io-characters-api-openapi.yml
- filename: openstela-io-deals-read-only-api-openapi.yml
  format: yaml
  label: OpenStela Deals (read-only) API
  slug: openstela-io-deals-read-only-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/openstela-io/openapi/openstela-io-deals-read-only-api-openapi.yml
- filename: openstela-io-messages-api-openapi.yml
  format: yaml
  label: OpenStela Messages API
  slug: openstela-io-messages-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/openstela-io/openapi/openstela-io-messages-api-openapi.yml
- filename: openstela-io-public-api-openapi.yml
  format: yaml
  label: OpenStela Public API
  slug: openstela-io-public-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/openstela-io/openapi/openstela-io-public-api-openapi.yml
- filename: openstela-io-verify-api-openapi.yml
  format: yaml
  label: OpenStela Verify API
  slug: openstela-io-verify-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/openstela-io/openapi/openstela-io-verify-api-openapi.yml
- filename: openstela-io-works-api-openapi.yml
  format: yaml
  label: OpenStela Works API
  slug: openstela-io-works-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/openstela-io/openapi/openstela-io-works-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: openstela.io
  spf: true
hosts:
- cert_expires: Feb 12 06:43:45 2027 GMT
  host: openstela.io
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: OpenStela Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for OpenStela, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: OpenStela
provider_slug: openstela-io
slug: openstela-io-domain-security
source_filename: openstela-io-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: openstela.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 12 06:43:45 2027 GMT\n  hsts: false\ndomains:\n- domain: openstela.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/openstela-io/security/openstela-io-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Blockchain
- Marketplace
- Digital Assets
- Creators
---
