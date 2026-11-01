---
api_specs:
- filename: credible-data-admin-api-reference-openapi-generated.yml
  format: yaml
  label: Credible Data Admin API Reference API
  slug: admin-api-reference-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/credible-data/openapi/_ae-authored/credible-data-admin-api-reference-openapi-generated.yml
- filename: credible-data-data-api-reference-openapi-generated.yml
  format: yaml
  label: Credible Data Data API Reference API
  slug: data-api-reference-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/credible-data/openapi/_ae-authored/credible-data-data-api-reference-openapi-generated.yml
- filename: credible-data-openapi-generated.yml
  format: yaml
  label: Credible Data API
  slug: full-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/credible-data/openapi/_ae-authored/credible-data-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: credibledata.com
  spf: true
hosts:
- cert_expires: Dec 12 00:43:31 2026 GMT
  host: www.credibledata.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Credible Data Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Credible Data, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Credible Data
provider_slug: credible-data
slug: credible-data-domain-security
source_filename: credible-data-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.credibledata.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 12 00:43:31 2026 GMT\n  hsts: false\ndomains:\n- domain: credibledata.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/credible-data/security/credible-data-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- AI
- Data Analytics
- Machine Learning
- Analytics Engine
- Platform
---
