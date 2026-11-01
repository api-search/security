---
api_specs:
- filename: classifier-dev-account-api-openapi.yml
  format: yaml
  label: classifier-dev Account API
  slug: classifier-dev-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/classifier-dev/openapi/classifier-dev-account-api-openapi.yml
- filename: classifier-dev-classifier-dev-api-openapi.yml
  format: yaml
  label: classifier-dev Classifier.dev API
  slug: classifier-dev-classifier-dev-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/classifier-dev/openapi/classifier-dev-classifier-dev-api-openapi.yml
- filename: classifier-dev-classify-api-openapi.yml
  format: yaml
  label: classifier-dev Classify API
  slug: classifier-dev-classify-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/classifier-dev/openapi/classifier-dev-classify-api-openapi.yml
- filename: classifier-dev-docs-api-openapi.yml
  format: yaml
  label: classifier-dev Docs API
  slug: classifier-dev-docs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/classifier-dev/openapi/classifier-dev-docs-api-openapi.yml
- filename: classifier-dev-feedback-api-openapi.yml
  format: yaml
  label: classifier-dev Feedback API
  slug: classifier-dev-feedback-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/classifier-dev/openapi/classifier-dev-feedback-api-openapi.yml
- filename: classifier-dev-subscribe-api-openapi.yml
  format: yaml
  label: classifier-dev Subscribe API
  slug: classifier-dev-subscribe-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/classifier-dev/openapi/classifier-dev-subscribe-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: classifier.dev
  spf: true
hosts:
- cert_expires: Jan  9 03:42:33 2027 GMT
  host: classifier.dev
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Classifier Dev Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for classifier-dev, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: classifier-dev
provider_slug: classifier-dev
slug: classifier-dev-domain-security
source_filename: classifier-dev-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: classifier.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  9 03:42:33 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: classifier.dev\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/classifier-dev/security/classifier-dev-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Machine Learning
- NLP
- Classification
- API
- OpenAPI
---
