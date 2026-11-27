---
api_specs:
- filename: bundle-social-analytics-api-openapi.yml
  format: yaml
  label: bundle.social Analytics API
  slug: bundle-social-analytics-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bundle-social/openapi/bundle-social-analytics-api-openapi.yml
- filename: bundle-social-app-api-openapi.yml
  format: yaml
  label: bundle.social App API
  slug: bundle-social-app-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bundle-social/openapi/bundle-social-app-api-openapi.yml
- filename: bundle-social-automation-api-openapi.yml
  format: yaml
  label: bundle.social Automation API
  slug: bundle-social-automation-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bundle-social/openapi/bundle-social-automation-api-openapi.yml
- filename: bundle-social-comment-api-openapi.yml
  format: yaml
  label: bundle.social Comment API
  slug: bundle-social-comment-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bundle-social/openapi/bundle-social-comment-api-openapi.yml
- filename: bundle-social-conversation-api-openapi.yml
  format: yaml
  label: bundle.social Conversation API
  slug: bundle-social-conversation-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bundle-social/openapi/bundle-social-conversation-api-openapi.yml
- filename: bundle-social-credit-api-openapi.yml
  format: yaml
  label: bundle.social Credit API
  slug: bundle-social-credit-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bundle-social/openapi/bundle-social-credit-api-openapi.yml
- filename: bundle-social-misc-api-openapi.yml
  format: yaml
  label: bundle.social Misc API
  slug: bundle-social-misc-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bundle-social/openapi/bundle-social-misc-api-openapi.yml
- filename: bundle-social-organization-api-openapi.yml
  format: yaml
  label: bundle.social Organization API
  slug: bundle-social-organization-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bundle-social/openapi/bundle-social-organization-api-openapi.yml
- filename: bundle-social-post-api-openapi.yml
  format: yaml
  label: bundle.social Post API
  slug: bundle-social-post-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bundle-social/openapi/bundle-social-post-api-openapi.yml
- filename: bundle-social-postcsv-api-openapi.yml
  format: yaml
  label: bundle.social Post CSV API
  slug: bundle-social-postcsv-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bundle-social/openapi/bundle-social-postcsv-api-openapi.yml
- filename: bundle-social-postimport-api-openapi.yml
  format: yaml
  label: bundle.social Post Import API
  slug: bundle-social-postimport-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bundle-social/openapi/bundle-social-postimport-api-openapi.yml
- filename: bundle-social-socialaccount-api-openapi.yml
  format: yaml
  label: bundle.social Social Account API
  slug: bundle-social-socialaccount-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bundle-social/openapi/bundle-social-socialaccount-api-openapi.yml
- filename: bundle-social-team-api-openapi.yml
  format: yaml
  label: bundle.social Team API
  slug: bundle-social-team-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bundle-social/openapi/bundle-social-team-api-openapi.yml
- filename: bundle-social-upload-api-openapi.yml
  format: yaml
  label: bundle.social Upload API
  slug: bundle-social-upload-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bundle-social/openapi/bundle-social-upload-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: bundle.social
  spf: true
hosts:
- cert_expires: Jan 15 01:01:37 2027 GMT
  host: bundle.social
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 25 18:33:02 2027 GMT
  host: info.bundle.social
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 25 18:33:02 2027 GMT
  host: api.bundle.social
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: bundle.social Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for bundle.social, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: bundle.social
provider_slug: bundle-social
slug: bundle-social-domain-security
source_filename: bundle-social-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: bundle.social\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 15 01:01:37 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: info.bundle.social\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 25 18:33:02 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.bundle.social\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 25 18:33:02 2027 GMT\n  hsts: null\ndomains:\n- domain: bundle.social\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/bundle-social/security/bundle-social-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Social
- Media
- Integration
- Unlimited
- Automation
---
