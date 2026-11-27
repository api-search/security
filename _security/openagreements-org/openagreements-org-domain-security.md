---
api_specs:
- filename: openagreements-org-llms-txt-api-openapi.yml
  format: yaml
  label: OpenAgreements Llms.txt API
  slug: openagreements-org-llms-txt-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/openagreements-org/openapi/openagreements-org-llms-txt-api-openapi.yml
- filename: openagreements-org-surveys-api-openapi.yml
  format: yaml
  label: OpenAgreements Surveys API
  slug: openagreements-org-surveys-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/openagreements-org/openapi/openagreements-org-surveys-api-openapi.yml
- filename: openagreements-org-well-known-api-openapi.yml
  format: yaml
  label: OpenAgreements .well Known API
  slug: openagreements-org-well-known-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/openagreements-org/openapi/openagreements-org-well-known-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 issue "sectigo.com"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: openagreements.org
  spf: true
hosts:
- cert_expires: Dec 28 12:38:02 2026 GMT
  host: openagreements.org
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: OpenAgreements Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for OpenAgreements, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: OpenAgreements
provider_slug: openagreements-org
slug: openagreements-org-domain-security
source_filename: openagreements-org-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: openagreements.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 28 12:38:02 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: openagreements.org\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"sectigo.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/openagreements-org/security/openagreements-org-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Legal
- Open Source
- Templates
- PracticeGuides
- Free
---
