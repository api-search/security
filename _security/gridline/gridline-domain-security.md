---
api_specs:
- filename: gridline-deepfake-api-openapi.yml
  format: yaml
  label: Gridlines Deepfake API
  slug: gridline-deepfake-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gridline/openapi/gridline-deepfake-api-openapi.yml
- filename: gridline-digilocker-api-openapi.yml
  format: yaml
  label: Gridlines Digilocker API
  slug: gridline-digilocker-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gridline/openapi/gridline-digilocker-api-openapi.yml
- filename: gridline-e-sign-api-openapi.yml
  format: yaml
  label: Gridlines E Sign API
  slug: gridline-e-sign-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gridline/openapi/gridline-e-sign-api-openapi.yml
- filename: gridline-face-api-api-openapi.yml
  format: yaml
  label: Gridlines Face API
  slug: gridline-face-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gridline/openapi/gridline-face-api-api-openapi.yml
- filename: gridline-individual-api-openapi.yml
  format: yaml
  label: Gridlines Individual API
  slug: gridline-individual-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gridline/openapi/gridline-individual-api-openapi.yml
- filename: gridline-liveness-api-openapi.yml
  format: yaml
  label: Gridlines Liveness API
  slug: gridline-liveness-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gridline/openapi/gridline-liveness-api-openapi.yml
- filename: gridline-pull-education-documents-api-openapi.yml
  format: yaml
  label: Gridlines Pull Education Documents API
  slug: gridline-pull-education-documents-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gridline/openapi/gridline-pull-education-documents-api-openapi.yml
- filename: gridline-uidai-ovse-api-openapi.yml
  format: yaml
  label: Gridlines UIDAI OVSE API
  slug: gridline-uidai-ovse-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gridline/openapi/gridline-uidai-ovse-api-openapi.yml
- filename: gridline-utility-api-openapi.yml
  format: yaml
  label: Gridlines Utility API
  slug: gridline-utility-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gridline/openapi/gridline-utility-api-openapi.yml
- filename: gridline-workflow-mgmt-api-openapi.yml
  format: yaml
  label: Gridlines Workflow Mgmt API
  slug: gridline-workflow-mgmt-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gridline/openapi/gridline-workflow-mgmt-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: gridlines.io
  spf: true
- caa:
  - 0 iodef "mailto:devops@stoplight.io"
  - 0 issue "cloudflare.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: stoplight.io
  spf: true
hosts:
- cert_expires: Apr  5 23:59:59 2027 GMT
  host: gridlines.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 26 05:33:25 2027 GMT
  host: gridlines.stoplight.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan  5 23:59:59 2027 GMT
  host: api.gridlines.io
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Gridline Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Gridlines, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Gridlines
provider_slug: gridline
slug: gridline-domain-security
source_filename: gridline-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: gridlines.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Apr  5 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: gridlines.stoplight.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 26 05:33:25 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.gridlines.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  5 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: gridlines.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: stoplight.io\n  dnssec: false\n  caa:\n  - 0 iodef \"mailto:devops@stoplight.io\"\n  - 0 issue \"cloudflare.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/gridline/security/gridline-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Onboarding
- IdentityVerification
- KYC
- eSigning
- FraudDetection
- VideoKYC
- DigitalOnboarding
- Fintech
---
