---
api_specs:
- filename: forgejo-activitypub-api-openapi.yml
  format: yaml
  label: Forgejo activitypub API
  slug: forgejo-activitypub-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/forgejo/refs/heads/main/openapi/forgejo-activitypub-api-openapi.yml
- filename: forgejo-admin-api-openapi.yml
  format: yaml
  label: Forgejo admin API
  slug: forgejo-admin-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/forgejo/refs/heads/main/openapi/forgejo-admin-api-openapi.yml
- filename: forgejo-issue-api-openapi.yml
  format: yaml
  label: Forgejo issue API
  slug: forgejo-issue-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/forgejo/refs/heads/main/openapi/forgejo-issue-api-openapi.yml
- filename: forgejo-miscellaneous-api-openapi.yml
  format: yaml
  label: Forgejo miscellaneous API
  slug: forgejo-miscellaneous-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/forgejo/refs/heads/main/openapi/forgejo-miscellaneous-api-openapi.yml
- filename: forgejo-notification-api-openapi.yml
  format: yaml
  label: Forgejo notification API
  slug: forgejo-notification-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/forgejo/refs/heads/main/openapi/forgejo-notification-api-openapi.yml
- filename: forgejo-organization-api-openapi.yml
  format: yaml
  label: Forgejo organization API
  slug: forgejo-organization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/forgejo/refs/heads/main/openapi/forgejo-organization-api-openapi.yml
- filename: forgejo-package-api-openapi.yml
  format: yaml
  label: Forgejo package API
  slug: forgejo-package-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/forgejo/refs/heads/main/openapi/forgejo-package-api-openapi.yml
- filename: forgejo-repository-api-openapi.yml
  format: yaml
  label: Forgejo repository API
  slug: forgejo-repository-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/forgejo/refs/heads/main/openapi/forgejo-repository-api-openapi.yml
- filename: forgejo-settings-api-openapi.yml
  format: yaml
  label: Forgejo settings API
  slug: forgejo-settings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/forgejo/refs/heads/main/openapi/forgejo-settings-api-openapi.yml
- filename: forgejo-user-api-openapi.yml
  format: yaml
  label: Forgejo user API
  slug: forgejo-user-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/forgejo/refs/heads/main/openapi/forgejo-user-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: forgejo.org
  spf: true
hosts:
- cert_expires: Aug 15 08:10:40 2026 GMT
  host: forgejo.org
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 29 04:49:46 2026 GMT
  host: code.forgejo.org
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Forgejo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Forgejo, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Forgejo
provider_slug: forgejo
slug: forgejo-domain-security
source_filename: forgejo-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: forgejo.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 15 08:10:40 2026 GMT\n  hsts: false\n- host: code.forgejo.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 04:49:46 2026 GMT\n  hsts: false\ndomains:\n- domain: forgejo.org\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/forgejo/refs/heads/main/security/forgejo-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Git
- Source Code Management
- Self-Hosted
- DevOps
- CI/CD
- Open-Source
- Forge
- Repositories
- Issues
- Pull Requests
---
