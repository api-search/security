---
api_specs:
- filename: imejis-io-analytics-api-openapi.yml
  format: yaml
  label: imejis-io Analytics API
  slug: imejis-io-analytics-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/imejis-io/openapi/imejis-io-analytics-api-openapi.yml
- filename: imejis-io-designs-api-openapi.yml
  format: yaml
  label: imejis-io Designs API
  slug: imejis-io-designs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/imejis-io/openapi/imejis-io-designs-api-openapi.yml
- filename: imejis-io-keys-api-openapi.yml
  format: yaml
  label: imejis-io Keys API
  slug: imejis-io-keys-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/imejis-io/openapi/imejis-io-keys-api-openapi.yml
- filename: imejis-io-render-api-openapi.yml
  format: yaml
  label: imejis-io Render API
  slug: imejis-io-render-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/imejis-io/openapi/imejis-io-render-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: imejis.io
  spf: true
hosts:
- cert_expires: Dec 25 10:32:37 2026 GMT
  host: imejis.io
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Imejis Io Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for imejis-io, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: imejis-io
provider_slug: imejis-io
slug: imejis-io-domain-security
source_filename: imejis-io-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: imejis.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 25 10:32:37 2026 GMT\n  hsts: false\ndomains:\n- domain: imejis.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/imejis-io/security/imejis-io-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
---
