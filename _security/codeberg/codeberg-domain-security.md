---
api_specs:
- filename: codeberg-miscellaneous-api-openapi.yml
  format: yaml
  label: Codeberg Miscellaneous API
  slug: codeberg-miscellaneous-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/codeberg/openapi/codeberg-miscellaneous-api-openapi.yml
- filename: codeberg-activitypub-api-openapi.yml
  format: yaml
  label: Codeberg Activitypub API
  slug: codeberg-activitypub-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/codeberg/openapi/codeberg-activitypub-api-openapi.yml
- filename: codeberg-admin-api-openapi.yml
  format: yaml
  label: Codeberg Admin API
  slug: codeberg-admin-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/codeberg/openapi/codeberg-admin-api-openapi.yml
- filename: codeberg-issue-api-openapi.yml
  format: yaml
  label: Codeberg Issue API
  slug: codeberg-issue-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/codeberg/openapi/codeberg-issue-api-openapi.yml
- filename: codeberg-notification-api-openapi.yml
  format: yaml
  label: Codeberg Notification API
  slug: codeberg-notification-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/codeberg/openapi/codeberg-notification-api-openapi.yml
- filename: codeberg-organization-api-openapi.yml
  format: yaml
  label: Codeberg Organization API
  slug: codeberg-organization-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/codeberg/openapi/codeberg-organization-api-openapi.yml
- filename: codeberg-package-api-openapi.yml
  format: yaml
  label: Codeberg Package API
  slug: codeberg-package-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/codeberg/openapi/codeberg-package-api-openapi.yml
- filename: codeberg-repository-api-openapi.yml
  format: yaml
  label: Codeberg Repository API
  slug: codeberg-repository-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/codeberg/openapi/codeberg-repository-api-openapi.yml
- filename: codeberg-settings-api-openapi.yml
  format: yaml
  label: Codeberg Settings API
  slug: codeberg-settings-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/codeberg/openapi/codeberg-settings-api-openapi.yml
- filename: codeberg-user-api-openapi.yml
  format: yaml
  label: Codeberg User API
  slug: codeberg-user-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/codeberg/openapi/codeberg-user-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: codeberg.org
  spf: true
  spf_record: v=spf1 mx a:mail.codeberg.eu -all
hosts:
- api_version_endpoint: https://codeberg.org/api/v1/version
  api_version_reported: 15.0.0-209-2308e484+gitea-1.22.0
  cert_expires: Oct  7 00:52:10 2026 GMT
  cert_issuer: Let's Encrypt
  host: codeberg.org
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 63072000
  hsts_preload: true
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Codeberg Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Codeberg, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Codeberg
provider_slug: codeberg
slug: codeberg-domain-security
source_filename: codeberg-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: codeberg.org\n  https: true\n  tls_version: TLSv1.3\n  cert_issuer: \"Let's Encrypt\"\n  cert_expires: Oct  7 00:52:10 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n  hsts_include_subdomains: true\n  hsts_preload: true\n  api_version_endpoint: https://codeberg.org/api/v1/version\n  api_version_reported: 15.0.0-209-2308e484+gitea-1.22.0\ndomains:\n- domain: codeberg.org\n  dnssec: true\n  caa: []\n  spf: true\n  spf_record: v=spf1 mx a:mail.codeberg.eu -all\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/codeberg/security/codeberg-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Code Hosting
- Version Control
- Git Hosting
- Repositories
- Pull Requests
- Issue Tracking
- Open Source
- Forgejo
- Non-Profit
---
