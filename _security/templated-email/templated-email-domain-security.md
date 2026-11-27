---
api_specs:
- filename: templated-email-accounts-api-openapi.yml
  format: yaml
  label: Templated Accounts API
  slug: templated-email-accounts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/templated-email/openapi/templated-email-accounts-api-openapi.yml
- filename: templated-email-ai-api-openapi.yml
  format: yaml
  label: Templated AI API
  slug: templated-email-ai-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/templated-email/openapi/templated-email-ai-api-openapi.yml
- filename: templated-email-api-keys-api-openapi.yml
  format: yaml
  label: Templated API Keys API
  slug: templated-email-api-keys-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/templated-email/openapi/templated-email-api-keys-api-openapi.yml
- filename: templated-email-brand-kit-api-openapi.yml
  format: yaml
  label: Templated Brand Kit API
  slug: templated-email-brand-kit-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/templated-email/openapi/templated-email-brand-kit-api-openapi.yml
- filename: templated-email-fonts-api-openapi.yml
  format: yaml
  label: Templated Fonts API
  slug: templated-email-fonts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/templated-email/openapi/templated-email-fonts-api-openapi.yml
- filename: templated-email-images-api-openapi.yml
  format: yaml
  label: Templated Images API
  slug: templated-email-images-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/templated-email/openapi/templated-email-images-api-openapi.yml
- filename: templated-email-integrations-api-openapi.yml
  format: yaml
  label: Templated Integrations API
  slug: templated-email-integrations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/templated-email/openapi/templated-email-integrations-api-openapi.yml
- filename: templated-email-members-api-openapi.yml
  format: yaml
  label: Templated Members API
  slug: templated-email-members-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/templated-email/openapi/templated-email-members-api-openapi.yml
- filename: templated-email-templates-api-openapi.yml
  format: yaml
  label: Templated Templates API
  slug: templated-email-templates-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/templated-email/openapi/templated-email-templates-api-openapi.yml
- filename: templated-email-testing-api-openapi.yml
  format: yaml
  label: Templated Testing API
  slug: templated-email-testing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/templated-email/openapi/templated-email-testing-api-openapi.yml
- filename: templated-email-unsplash-api-openapi.yml
  format: yaml
  label: Templated Unsplash API
  slug: templated-email-unsplash-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/templated-email/openapi/templated-email-unsplash-api-openapi.yml
- filename: templated-email-subaccounts-api-openapi.yml
  format: yaml
  label: Templated Subaccounts API
  slug: templated-email-subaccounts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/templated-email/openapi/templated-email-subaccounts-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dns_aid:
    checked: '2026-11-26'
    published: false
  dnssec: false
  domain: templated.email
  spf: true
hosts:
- cert_expires: Dec 29 02:40:00 2026 GMT
  host: templated.email
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Templated Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Templated, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Templated
provider_slug: templated-email
slug: templated-email-domain-security
source_filename: templated-email-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: templated.email\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 29 02:40:00 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: templated.email\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n  dns_aid:\n    checked: '2026-11-26'\n    published: false\n"
source_yaml_url: https://artifacts.apis.io/templated-email/security/templated-email-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Email
- AI
- No-code
- Marketing
---
