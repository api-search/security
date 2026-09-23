---
api_specs:
- filename: gogs-administration-api-openapi.yml
  format: yaml
  label: Gogs Administration API
  slug: gogs-administration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gogs/refs/heads/main/openapi/gogs-administration-api-openapi.yml
- filename: gogs-collaborators-and-deploy-keys-api-openapi.yml
  format: yaml
  label: Gogs Collaborators and Deploy Keys API
  slug: gogs-collaborators-and-deploy-keys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gogs/refs/heads/main/openapi/gogs-collaborators-and-deploy-keys-api-openapi.yml
- filename: gogs-issues-api-openapi.yml
  format: yaml
  label: Gogs Issues API
  slug: gogs-issues-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gogs/refs/heads/main/openapi/gogs-issues-api-openapi.yml
- filename: gogs-miscellaneous-api-openapi.yml
  format: yaml
  label: Gogs Miscellaneous API
  slug: gogs-miscellaneous-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gogs/refs/heads/main/openapi/gogs-miscellaneous-api-openapi.yml
- filename: gogs-organizations-api-openapi.yml
  format: yaml
  label: Gogs Organizations API
  slug: gogs-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gogs/refs/heads/main/openapi/gogs-organizations-api-openapi.yml
- filename: gogs-releases-api-openapi.yml
  format: yaml
  label: Gogs Releases API
  slug: gogs-releases-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gogs/refs/heads/main/openapi/gogs-releases-api-openapi.yml
- filename: gogs-repositories-api-openapi.yml
  format: yaml
  label: Gogs Repositories API
  slug: gogs-repositories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gogs/refs/heads/main/openapi/gogs-repositories-api-openapi.yml
- filename: gogs-users-api-openapi.yml
  format: yaml
  label: Gogs Users API
  slug: gogs-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gogs/refs/heads/main/openapi/gogs-users-api-openapi.yml
- filename: gogs-webhooks-api-openapi.yml
  format: yaml
  label: Gogs Webhooks API
  slug: gogs-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gogs/refs/heads/main/openapi/gogs-webhooks-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: true
  domain: gogs.io
  spf: true
hosts:
- cert_expires: Dec  1 18:43:57 2026 GMT
  host: gogs.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Gogs Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Gogs, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC absent.'
provider_name: Gogs
provider_slug: gogs
slug: gogs-domain-security
source_filename: gogs-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: gogs.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  1 18:43:57 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: gogs.io\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gogs/refs/heads/main/security/gogs-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC
tags:
- Company
- Git
- Self-Hosted
- Open-Source
- Go
---
