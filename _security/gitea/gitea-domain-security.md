---
api_specs:
- filename: gitea-admin-api-openapi.yml
  format: yaml
  label: Gitea admin API
  slug: gitea-admin-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gitea/refs/heads/main/openapi/gitea-admin-api-openapi.yml
- filename: gitea-issue-api-openapi.yml
  format: yaml
  label: Gitea issue API
  slug: gitea-issue-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gitea/refs/heads/main/openapi/gitea-issue-api-openapi.yml
- filename: gitea-miscellaneous-api-openapi.yml
  format: yaml
  label: Gitea miscellaneous API
  slug: gitea-miscellaneous-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gitea/refs/heads/main/openapi/gitea-miscellaneous-api-openapi.yml
- filename: gitea-notification-api-openapi.yml
  format: yaml
  label: Gitea notification API
  slug: gitea-notification-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gitea/refs/heads/main/openapi/gitea-notification-api-openapi.yml
- filename: gitea-organization-api-openapi.yml
  format: yaml
  label: Gitea organization API
  slug: gitea-organization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gitea/refs/heads/main/openapi/gitea-organization-api-openapi.yml
- filename: gitea-package-api-openapi.yml
  format: yaml
  label: Gitea package API
  slug: gitea-package-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gitea/refs/heads/main/openapi/gitea-package-api-openapi.yml
- filename: gitea-repository-api-openapi.yml
  format: yaml
  label: Gitea repository API
  slug: gitea-repository-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gitea/refs/heads/main/openapi/gitea-repository-api-openapi.yml
- filename: gitea-settings-api-openapi.yml
  format: yaml
  label: Gitea settings API
  slug: gitea-settings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gitea/refs/heads/main/openapi/gitea-settings-api-openapi.yml
- filename: gitea-user-api-openapi.yml
  format: yaml
  label: Gitea user API
  slug: gitea-user-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gitea/refs/heads/main/openapi/gitea-user-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: gitea.com
  spf: true
hosts:
- cert_expires: Sep 25 23:44:39 2026 GMT
  host: about.gitea.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 23 23:59:59 2026 GMT
  host: docs.gitea.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 18 23:59:59 2026 GMT
  host: gitea.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Gitea Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Gitea, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Gitea
provider_slug: gitea
slug: gitea-domain-security
source_filename: gitea-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: about.gitea.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 25 23:44:39 2026 GMT\n  hsts: false\n- host: docs.gitea.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 23 23:59:59 2026 GMT\n  hsts: false\n- host: gitea.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 18 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: gitea.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gitea/refs/heads/main/security/gitea-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Git
- Source Control
- DevOps
- CI/CD
- Code Hosting
- Open-Source
- Self-Hosted
- Package Registry
- Issue Tracking
- Pull Requests
---
