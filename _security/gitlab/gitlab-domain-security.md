---
api_specs:
- filename: gitlab-api-v4-groups-openapi-original.yml
  format: yaml
  label: GitLab Groups API
  slug: apiv4groups
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gitlab/refs/heads/main/openapi/gitlab-api-v4-groups-openapi-original.yml
- filename: gitlab-api-v4-projects-openapi-original.yml
  format: yaml
  label: GitLab Projects API
  slug: apiv4projects
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gitlab/refs/heads/main/openapi/gitlab-api-v4-projects-openapi-original.yml
- filename: gitlab-api-v4-admin-openapi-original.yml
  format: yaml
  label: GitLab Admin API
  slug: apiv4admin
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gitlab/refs/heads/main/openapi/gitlab-api-v4-admin-openapi-original.yml
- filename: gitlab-api-v4-applications-openapi-original.yml
  format: yaml
  label: GitLab Applications API
  slug: apiv4applications
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gitlab/refs/heads/main/openapi/gitlab-api-v4-applications-openapi-original.yml
- filename: gitlab-api-v4-avatar-openapi-original.yml
  format: yaml
  label: GitLab Avatar API
  slug: apiv4avatar
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gitlab/refs/heads/main/openapi/gitlab-api-v4-avatar-openapi-original.yml
- filename: gitlab-api-v4-broadcast-messages-openapi-original.yml
  format: yaml
  label: GitLab Broadcast Messages API
  slug: apiv4broadcast-messages
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gitlab/refs/heads/main/openapi/gitlab-api-v4-broadcast-messages-openapi-original.yml
- filename: gitlab-api-v4-bulk-imports-openapi-original.yml
  format: yaml
  label: GitLab Bulk Imports API
  slug: apiv4bulk-imports
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gitlab/refs/heads/main/openapi/gitlab-api-v4-bulk-imports-openapi-original.yml
- filename: gitlab-api-v4-application-openapi-original.yml
  format: yaml
  label: GitLab Application Settings API
  slug: apiv4application
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gitlab/refs/heads/main/openapi/gitlab-api-v4-application-openapi-original.yml
- filename: gitlab-api-v4-metadata-openapi-original.yml
  format: yaml
  label: GitLab Metadata API
  slug: apiv4metadata
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gitlab/refs/heads/main/openapi/gitlab-api-v4-metadata-openapi-original.yml
- filename: gitlab-api-v4-version-openapi-original.yml
  format: yaml
  label: GitLab Version API
  slug: apiv4version
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gitlab/refs/heads/main/openapi/gitlab-api-v4-version-openapi-original.yml
- filename: gitlab-openapi-original.yml
  format: yaml
  label: GitLab REST API
  slug: gitlab-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gitlab/refs/heads/main/openapi/gitlab-openapi-original.yml
- filename: gitlab-oauth2-openapi.yml
  format: yaml
  label: GitLab OAuth 2.0 API
  slug: gitlab-oauth2-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gitlab/refs/heads/main/openapi/gitlab-oauth2-openapi.yml
- filename: gitlab-webhooks-openapi.yml
  format: yaml
  label: GitLab Webhooks
  slug: gitlab-webhooks
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gitlab/refs/heads/main/openapi/gitlab-webhooks-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "amazon.com"
  - 0 issue "amazonaws.com"
  - 0 issue "amazontrust.com"
  - 0 issue "awstrust.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: gitlab.com
  spf: true
hosts:
- cert_expires: Aug 18 18:49:38 2026 GMT
  host: about.gitlab.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 18 12:39:50 2026 GMT
  host: docs.gitlab.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  7 17:32:43 2026 GMT
  host: developer.gitlab.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Gitlab Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for GitLab, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: GitLab
provider_slug: gitlab
slug: gitlab-domain-security
source_filename: gitlab-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: about.gitlab.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 18 18:49:38 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.gitlab.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 18 12:39:50 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developer.gitlab.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  7 17:32:43 2026 GMT\n  hsts: false\ndomains:\n- domain: gitlab.com\n  dnssec: false\n  caa:\n  - 0 issue \"amazon.com\"\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"amazontrust.com\"\n  - 0 issue \"awstrust.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gitlab/refs/heads/main/security/gitlab-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Code
- Platform
- Software Development
- Source Control
---
