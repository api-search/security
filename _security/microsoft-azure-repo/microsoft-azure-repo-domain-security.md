---
api_specs:
- filename: microsoft-azure-repo-commits-api-openapi.yml
  format: yaml
  label: Azure Repos Commits API
  slug: microsoft-azure-repo-commits-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure-repo/refs/heads/main/openapi/microsoft-azure-repo-commits-api-openapi.yml
- filename: microsoft-azure-repo-items-api-openapi.yml
  format: yaml
  label: Azure Repos Items API
  slug: microsoft-azure-repo-items-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure-repo/refs/heads/main/openapi/microsoft-azure-repo-items-api-openapi.yml
- filename: microsoft-azure-repo-pull-request-reviewers-api-openapi.yml
  format: yaml
  label: Azure Repos Pull Request Reviewers API
  slug: microsoft-azure-repo-pull-request-reviewers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure-repo/refs/heads/main/openapi/microsoft-azure-repo-pull-request-reviewers-api-openapi.yml
- filename: microsoft-azure-repo-pull-request-threads-api-openapi.yml
  format: yaml
  label: Azure Repos Pull Request Threads API
  slug: microsoft-azure-repo-pull-request-threads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure-repo/refs/heads/main/openapi/microsoft-azure-repo-pull-request-threads-api-openapi.yml
- filename: microsoft-azure-repo-pull-requests-api-openapi.yml
  format: yaml
  label: Azure Repos Pull Requests API
  slug: microsoft-azure-repo-pull-requests-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure-repo/refs/heads/main/openapi/microsoft-azure-repo-pull-requests-api-openapi.yml
- filename: microsoft-azure-repo-pushes-api-openapi.yml
  format: yaml
  label: Azure Repos Pushes API
  slug: microsoft-azure-repo-pushes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure-repo/refs/heads/main/openapi/microsoft-azure-repo-pushes-api-openapi.yml
- filename: microsoft-azure-repo-refs-api-openapi.yml
  format: yaml
  label: Azure Repos Refs API
  slug: microsoft-azure-repo-refs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure-repo/refs/heads/main/openapi/microsoft-azure-repo-refs-api-openapi.yml
- filename: microsoft-azure-repo-repositories-api-openapi.yml
  format: yaml
  label: Azure Repos Repositories API
  slug: microsoft-azure-repo-repositories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure-repo/refs/heads/main/openapi/microsoft-azure-repo-repositories-api-openapi.yml
- filename: microsoft-azure-repo-stats-api-openapi.yml
  format: yaml
  label: Azure Repos Stats API
  slug: microsoft-azure-repo-stats-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure-repo/refs/heads/main/openapi/microsoft-azure-repo-stats-api-openapi.yml
description: ''
domains:
- caa:
  - 0 contactemail "caarecordaware@microsoft.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: microsoft.com
  spf: true
hosts:
- cert_expires: Dec 11 02:26:09 2026 GMT
  host: learn.microsoft.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 24 22:04:48 2026 GMT
  host: azure.microsoft.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 10 06:59:10 2026 GMT
  host: docs.microsoft.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Microsoft Azure Repo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Azure Repos, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Azure Repos
provider_slug: microsoft-azure-repo
slug: microsoft-azure-repo-domain-security
source_filename: microsoft-azure-repo-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: learn.microsoft.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 11 02:26:09 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: azure.microsoft.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 24 22:04:48 2026 GMT\n  hsts: null\n- host: docs.microsoft.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 10 06:59:10 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: microsoft.com\n  dnssec: false\n  caa:\n  - 0 contactemail \"caarecordaware@microsoft.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure-repo/refs/heads/main/security/microsoft-azure-repo-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- DevOps
- Git
- Repositories
- Source Control
- TFVC
- Version Control
---
