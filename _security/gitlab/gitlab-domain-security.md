---
api_specs:
- filename: gitlab-admin-api-openapi.yml
  format: yaml
  label: GitLab Admin API
  slug: gitlab-admin-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gitlab/refs/heads/main/openapi/gitlab-admin-api-openapi.yml
- filename: gitlab-application-api-openapi.yml
  format: yaml
  label: GitLab Application API
  slug: gitlab-application-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gitlab/refs/heads/main/openapi/gitlab-application-api-openapi.yml
- filename: gitlab-applications-api-openapi.yml
  format: yaml
  label: GitLab Applications API
  slug: gitlab-applications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gitlab/refs/heads/main/openapi/gitlab-applications-api-openapi.yml
- filename: gitlab-authorization-api-openapi.yml
  format: yaml
  label: GitLab Authorization API
  slug: gitlab-authorization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gitlab/refs/heads/main/openapi/gitlab-authorization-api-openapi.yml
- filename: gitlab-avatar-api-openapi.yml
  format: yaml
  label: GitLab Avatar API
  slug: gitlab-avatar-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gitlab/refs/heads/main/openapi/gitlab-avatar-api-openapi.yml
- filename: gitlab-broadcast-messages-api-openapi.yml
  format: yaml
  label: GitLab Broadcast Messages API
  slug: gitlab-broadcast-messages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gitlab/refs/heads/main/openapi/gitlab-broadcast-messages-api-openapi.yml
- filename: gitlab-bulk-imports-api-openapi.yml
  format: yaml
  label: GitLab Bulk Imports API
  slug: gitlab-bulk-imports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gitlab/refs/heads/main/openapi/gitlab-bulk-imports-api-openapi.yml
- filename: gitlab-groups-api-openapi.yml
  format: yaml
  label: GitLab Groups API
  slug: gitlab-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gitlab/refs/heads/main/openapi/gitlab-groups-api-openapi.yml
- filename: gitlab-metadata-api-openapi.yml
  format: yaml
  label: GitLab Metadata API
  slug: gitlab-metadata-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gitlab/refs/heads/main/openapi/gitlab-metadata-api-openapi.yml
- filename: gitlab-project-webhooks-api-openapi.yml
  format: yaml
  label: GitLab Project Webhooks API
  slug: gitlab-project-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gitlab/refs/heads/main/openapi/gitlab-project-webhooks-api-openapi.yml
- filename: gitlab-projects-api-openapi.yml
  format: yaml
  label: GitLab Projects API
  slug: gitlab-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gitlab/refs/heads/main/openapi/gitlab-projects-api-openapi.yml
- filename: gitlab-tokens-api-openapi.yml
  format: yaml
  label: GitLab Tokens API
  slug: gitlab-tokens-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gitlab/refs/heads/main/openapi/gitlab-tokens-api-openapi.yml
- filename: gitlab-user-info-api-openapi.yml
  format: yaml
  label: GitLab User Info API
  slug: gitlab-user-info-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gitlab/refs/heads/main/openapi/gitlab-user-info-api-openapi.yml
- filename: gitlab-version-api-openapi.yml
  format: yaml
  label: GitLab Version API
  slug: gitlab-version-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gitlab/refs/heads/main/openapi/gitlab-version-api-openapi.yml
- filename: gitlab-webhook-configuration-api-openapi.yml
  format: yaml
  label: GitLab Webhook Configuration API
  slug: gitlab-webhook-configuration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gitlab/refs/heads/main/openapi/gitlab-webhook-configuration-api-openapi.yml
- filename: gitlab-webhook-events-api-openapi.yml
  format: yaml
  label: GitLab Webhook Events API
  slug: gitlab-webhook-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gitlab/refs/heads/main/openapi/gitlab-webhook-events-api-openapi.yml
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
