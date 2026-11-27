---
api_specs:
- filename: octolens-com-agency-api-openapi.yml
  format: yaml
  label: Octolens Agency API
  slug: octolens-com-agency-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/octolens-com/openapi/octolens-com-agency-api-openapi.yml
- filename: octolens-com-ai-api-openapi.yml
  format: yaml
  label: Octolens AI API
  slug: octolens-com-ai-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/octolens-com/openapi/octolens-com-ai-api-openapi.yml
- filename: octolens-com-analytics-api-openapi.yml
  format: yaml
  label: Octolens Analytics API
  slug: octolens-com-analytics-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/octolens-com/openapi/octolens-com-analytics-api-openapi.yml
- filename: octolens-com-attention-api-openapi.yml
  format: yaml
  label: Octolens Attention API
  slug: octolens-com-attention-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/octolens-com/openapi/octolens-com-attention-api-openapi.yml
- filename: octolens-com-auth-api-openapi.yml
  format: yaml
  label: Octolens Auth API
  slug: octolens-com-auth-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/octolens-com/openapi/octolens-com-auth-api-openapi.yml
- filename: octolens-com-feedback-api-openapi.yml
  format: yaml
  label: Octolens Feedback API
  slug: octolens-com-feedback-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/octolens-com/openapi/octolens-com-feedback-api-openapi.yml
- filename: octolens-com-feeds-api-openapi.yml
  format: yaml
  label: Octolens Feeds API
  slug: octolens-com-feeds-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/octolens-com/openapi/octolens-com-feeds-api-openapi.yml
- filename: octolens-com-filters-api-openapi.yml
  format: yaml
  label: Octolens Filters API
  slug: octolens-com-filters-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/octolens-com/openapi/octolens-com-filters-api-openapi.yml
- filename: octolens-com-integrations-api-openapi.yml
  format: yaml
  label: Octolens Integrations API
  slug: octolens-com-integrations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/octolens-com/openapi/octolens-com-integrations-api-openapi.yml
- filename: octolens-com-keywords-api-openapi.yml
  format: yaml
  label: Octolens Keywords API
  slug: octolens-com-keywords-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/octolens-com/openapi/octolens-com-keywords-api-openapi.yml
- filename: octolens-com-members-api-openapi.yml
  format: yaml
  label: Octolens Members API
  slug: octolens-com-members-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/octolens-com/openapi/octolens-com-members-api-openapi.yml
- filename: octolens-com-mentions-api-openapi.yml
  format: yaml
  label: Octolens Mentions API
  slug: octolens-com-mentions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/octolens-com/openapi/octolens-com-mentions-api-openapi.yml
- filename: octolens-com-notifications-api-openapi.yml
  format: yaml
  label: Octolens Notifications API
  slug: octolens-com-notifications-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/octolens-com/openapi/octolens-com-notifications-api-openapi.yml
- filename: octolens-com-onboarding-api-openapi.yml
  format: yaml
  label: Octolens Onboarding API
  slug: octolens-com-onboarding-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/octolens-com/openapi/octolens-com-onboarding-api-openapi.yml
- filename: octolens-com-organization-api-openapi.yml
  format: yaml
  label: Octolens Organization API
  slug: octolens-com-organization-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/octolens-com/openapi/octolens-com-organization-api-openapi.yml
- filename: octolens-com-search-api-openapi.yml
  format: yaml
  label: Octolens Search API
  slug: octolens-com-search-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/octolens-com/openapi/octolens-com-search-api-openapi.yml
- filename: octolens-com-setup-api-openapi.yml
  format: yaml
  label: Octolens Setup API
  slug: octolens-com-setup-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/octolens-com/openapi/octolens-com-setup-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 issue "sectigo.com"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: octolens.com
  spf: true
hosts:
- cert_expires: Jan 23 05:13:08 2027 GMT
  host: octolens.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Octolens Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Octolens, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Octolens
provider_slug: octolens-com
slug: octolens-com-domain-security
source_filename: octolens-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: octolens.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 23 05:13:08 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: octolens.com\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"sectigo.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/octolens-com/security/octolens-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Social Listening
- Artificial Intelligence
- Marketing
- Analytics
---
