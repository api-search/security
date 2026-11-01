---
api_specs:
- filename: emailverifier-dev-domains-api-openapi.yml
  format: yaml
  label: emailverifier-dev Domains API
  slug: emailverifier-dev-domains-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/emailverifier-dev/openapi/emailverifier-dev-domains-api-openapi.yml
- filename: emailverifier-dev-usage-api-openapi.yml
  format: yaml
  label: emailverifier-dev Usage API
  slug: emailverifier-dev-usage-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/emailverifier-dev/openapi/emailverifier-dev-usage-api-openapi.yml
- filename: emailverifier-dev-verification-api-openapi.yml
  format: yaml
  label: emailverifier-dev Verification API
  slug: emailverifier-dev-verification-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/emailverifier-dev/openapi/emailverifier-dev-verification-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: emailverifier.dev
  spf: true
hosts:
- cert_expires: Jan 21 12:27:29 2027 GMT
  host: emailverifier.dev
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Emailverifier Dev Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for emailverifier-dev, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: emailverifier-dev
provider_slug: emailverifier-dev
slug: emailverifier-dev-domain-security
source_filename: emailverifier-dev-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: emailverifier.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 21 12:27:29 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: emailverifier.dev\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/emailverifier-dev/security/emailverifier-dev-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Email
- Verification
- API
- SaaS
- DataQuality
---
