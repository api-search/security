---
api_specs:
- filename: arcnm-io-calculations-api-openapi.yml
  format: yaml
  label: ARCNM Calculations API
  slug: arcnm-io-calculations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/arcnm-io/openapi/arcnm-io-calculations-api-openapi.yml
- filename: arcnm-io-calibration-api-openapi.yml
  format: yaml
  label: ARCNM Calibration API
  slug: arcnm-io-calibration-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/arcnm-io/openapi/arcnm-io-calibration-api-openapi.yml
- filename: arcnm-io-datasets-api-openapi.yml
  format: yaml
  label: ARCNM Datasets API
  slug: arcnm-io-datasets-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/arcnm-io/openapi/arcnm-io-datasets-api-openapi.yml
- filename: arcnm-io-environments-api-openapi.yml
  format: yaml
  label: ARCNM Environments API
  slug: arcnm-io-environments-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/arcnm-io/openapi/arcnm-io-environments-api-openapi.yml
- filename: arcnm-io-folders-api-openapi.yml
  format: yaml
  label: ARCNM Folders API
  slug: arcnm-io-folders-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/arcnm-io/openapi/arcnm-io-folders-api-openapi.yml
- filename: arcnm-io-geometry-api-openapi.yml
  format: yaml
  label: ARCNM Geometry API
  slug: arcnm-io-geometry-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/arcnm-io/openapi/arcnm-io-geometry-api-openapi.yml
- filename: arcnm-io-import-api-openapi.yml
  format: yaml
  label: ARCNM Import API
  slug: arcnm-io-import-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/arcnm-io/openapi/arcnm-io-import-api-openapi.yml
- filename: arcnm-io-machine-library-api-openapi.yml
  format: yaml
  label: ARCNM Machine Library API
  slug: arcnm-io-machine-library-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/arcnm-io/openapi/arcnm-io-machine-library-api-openapi.yml
- filename: arcnm-io-machines-api-openapi.yml
  format: yaml
  label: ARCNM Machines API
  slug: arcnm-io-machines-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/arcnm-io/openapi/arcnm-io-machines-api-openapi.yml
- filename: arcnm-io-materials-api-openapi.yml
  format: yaml
  label: ARCNM Materials API
  slug: arcnm-io-materials-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/arcnm-io/openapi/arcnm-io-materials-api-openapi.yml
- filename: arcnm-io-nesting-api-openapi.yml
  format: yaml
  label: ARCNM Nesting API
  slug: arcnm-io-nesting-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/arcnm-io/openapi/arcnm-io-nesting-api-openapi.yml
- filename: arcnm-io-parts-api-openapi.yml
  format: yaml
  label: ARCNM Parts API
  slug: arcnm-io-parts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/arcnm-io/openapi/arcnm-io-parts-api-openapi.yml
- filename: arcnm-io-remnants-api-openapi.yml
  format: yaml
  label: ARCNM Remnants API
  slug: arcnm-io-remnants-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/arcnm-io/openapi/arcnm-io-remnants-api-openapi.yml
- filename: arcnm-io-subcontractors-api-openapi.yml
  format: yaml
  label: ARCNM Subcontractors API
  slug: arcnm-io-subcontractors-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/arcnm-io/openapi/arcnm-io-subcontractors-api-openapi.yml
- filename: arcnm-io-tools-api-openapi.yml
  format: yaml
  label: ARCNM Tools API
  slug: arcnm-io-tools-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/arcnm-io/openapi/arcnm-io-tools-api-openapi.yml
- filename: arcnm-io-upload-links-api-openapi.yml
  format: yaml
  label: ARCNM Upload Links API
  slug: arcnm-io-upload-links-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/arcnm-io/openapi/arcnm-io-upload-links-api-openapi.yml
- filename: arcnm-io-uploads-api-openapi.yml
  format: yaml
  label: ARCNM Uploads API
  slug: arcnm-io-uploads-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/arcnm-io/openapi/arcnm-io-uploads-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: arcnm.io
  spf: true
hosts:
- cert_expires: Dec 22 18:46:06 2026 GMT
  host: arcnm.io
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: ARCNM Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ARCNM, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: ARCNM
provider_slug: arcnm-io
slug: arcnm-io-domain-security
source_filename: arcnm-io-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-01'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: arcnm.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 22 18:46:06 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: arcnm.io\n  dnssec: false\n  caa:\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/arcnm-io/security/arcnm-io-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Manufacturing
- Costing
- CAD
- Engineering
---
