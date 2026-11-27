---
api_specs:
- filename: zvid-io-api-keys-api-openapi.yml
  format: yaml
  label: zvid-io API Keys API
  slug: zvid-io-api-keys-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/zvid-io/openapi/zvid-io-api-keys-api-openapi.yml
- filename: zvid-io-authoring-api-openapi.yml
  format: yaml
  label: zvid-io Authoring API
  slug: zvid-io-authoring-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/zvid-io/openapi/zvid-io-authoring-api-openapi.yml
- filename: zvid-io-bulk-render-api-openapi.yml
  format: yaml
  label: zvid-io Bulk Render API
  slug: zvid-io-bulk-render-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/zvid-io/openapi/zvid-io-bulk-render-api-openapi.yml
- filename: zvid-io-credits-api-openapi.yml
  format: yaml
  label: zvid-io Credits API
  slug: zvid-io-credits-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/zvid-io/openapi/zvid-io-credits-api-openapi.yml
- filename: zvid-io-library-api-openapi.yml
  format: yaml
  label: zvid-io Library API
  slug: zvid-io-library-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/zvid-io/openapi/zvid-io-library-api-openapi.yml
- filename: zvid-io-projects-api-openapi.yml
  format: yaml
  label: zvid-io Projects API
  slug: zvid-io-projects-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/zvid-io/openapi/zvid-io-projects-api-openapi.yml
- filename: zvid-io-render-api-openapi.yml
  format: yaml
  label: zvid-io Render API
  slug: zvid-io-render-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/zvid-io/openapi/zvid-io-render-api-openapi.yml
- filename: zvid-io-stock-api-openapi.yml
  format: yaml
  label: zvid-io Stock API
  slug: zvid-io-stock-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/zvid-io/openapi/zvid-io-stock-api-openapi.yml
- filename: zvid-io-templates-api-openapi.yml
  format: yaml
  label: zvid-io Templates API
  slug: zvid-io-templates-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/zvid-io/openapi/zvid-io-templates-api-openapi.yml
- filename: zvid-io-uploads-api-openapi.yml
  format: yaml
  label: zvid-io Uploads API
  slug: zvid-io-uploads-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/zvid-io/openapi/zvid-io-uploads-api-openapi.yml
- filename: zvid-io-user-api-openapi.yml
  format: yaml
  label: zvid-io User API
  slug: zvid-io-user-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/zvid-io/openapi/zvid-io-user-api-openapi.yml
- filename: zvid-io-webhooks-api-openapi.yml
  format: yaml
  label: zvid-io Webhooks API
  slug: zvid-io-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/zvid-io/openapi/zvid-io-webhooks-api-openapi.yml
- filename: zvid-io-zvid-api-api-openapi.yml
  format: yaml
  label: zvid-io Zvid API
  slug: zvid-io-zvid-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/zvid-io/openapi/zvid-io-zvid-api-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "ssl.com"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "globalsign.com"
  - 0 issuewild "letsencrypt.org"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: zvid.io
  spf: true
hosts:
- cert_expires: Jan 13 09:26:11 2027 GMT
  host: zvid.io
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: zvid-io Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for zvid-io, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: zvid-io
provider_slug: zvid-io
slug: zvid-io-domain-security
source_filename: zvid-io-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: zvid.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 13 09:26:11 2027 GMT\n  hsts: false\ndomains:\n- domain: zvid.io\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"globalsign.com\"\n  - 0 issuewild \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/zvid-io/security/zvid-io-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Video
- Automation
- Media
---
