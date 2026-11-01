---
api_specs:
- filename: coderpad-account-api-openapi.yml
  format: yaml
  label: CoderPad Account API
  slug: coderpad-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coderpad/openapi/coderpad-account-api-openapi.yml
- filename: coderpad-campaigns-api-openapi.yml
  format: yaml
  label: CoderPad Campaigns API
  slug: coderpad-campaigns-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coderpad/openapi/coderpad-campaigns-api-openapi.yml
- filename: coderpad-me-api-openapi.yml
  format: yaml
  label: CoderPad Me API
  slug: coderpad-me-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coderpad/openapi/coderpad-me-api-openapi.yml
- filename: coderpad-organization-api-openapi.yml
  format: yaml
  label: CoderPad Organization API
  slug: coderpad-organization-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coderpad/openapi/coderpad-organization-api-openapi.yml
- filename: coderpad-pad-environments-api-openapi.yml
  format: yaml
  label: CoderPad Pad environments API
  slug: coderpad-pad-environments-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coderpad/openapi/coderpad-pad-environments-api-openapi.yml
- filename: coderpad-pads-api-openapi.yml
  format: yaml
  label: CoderPad Pads API
  slug: coderpad-pads-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coderpad/openapi/coderpad-pads-api-openapi.yml
- filename: coderpad-question-variants-api-openapi.yml
  format: yaml
  label: CoderPad Question variants API
  slug: coderpad-question-variants-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coderpad/openapi/coderpad-question-variants-api-openapi.yml
- filename: coderpad-questions-api-openapi.yml
  format: yaml
  label: CoderPad Questions API
  slug: coderpad-questions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coderpad/openapi/coderpad-questions-api-openapi.yml
- filename: coderpad-temporaryfile-api-openapi.yml
  format: yaml
  label: CoderPad Temporary File API
  slug: coderpad-temporaryfile-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coderpad/openapi/coderpad-temporaryfile-api-openapi.yml
- filename: coderpad-tests-api-openapi.yml
  format: yaml
  label: CoderPad Tests API
  slug: coderpad-tests-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coderpad/openapi/coderpad-tests-api-openapi.yml
- filename: coderpad-webhook-api-openapi.yml
  format: yaml
  label: CoderPad Webhook API
  slug: coderpad-webhook-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coderpad/openapi/coderpad-webhook-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  - 0 issue "amazontrust.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: coderpad.io
  spf: true
hosts:
- cert_expires: Jan 20 16:17:36 2027 GMT
  host: coderpad.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Coderpad Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for CoderPad, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: CoderPad
provider_slug: coderpad
slug: coderpad-domain-security
source_filename: coderpad-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-27'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: coderpad.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 20 16:17:36 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: coderpad.io\n  dnssec: true\n  caa:\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"amazontrust.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/coderpad/security/coderpad-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- AI
- Hiring
- TechnicalAssessment
- InterviewPlatform
---
