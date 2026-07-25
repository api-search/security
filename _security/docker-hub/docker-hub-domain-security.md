---
api_specs:
- filename: docker-hub-access-tokens-api-openapi.yml
  format: yaml
  label: Docker Hub access-tokens API
  slug: docker-hub-access-tokens-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/docker-hub/refs/heads/main/openapi/docker-hub-access-tokens-api-openapi.yml
- filename: docker-hub-audit-logs-api-openapi.yml
  format: yaml
  label: Docker Hub audit-logs API
  slug: docker-hub-audit-logs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/docker-hub/refs/heads/main/openapi/docker-hub-audit-logs-api-openapi.yml
- filename: docker-hub-authentication-api-api-openapi.yml
  format: yaml
  label: Docker Hub authentication-api API
  slug: docker-hub-authentication-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/docker-hub/refs/heads/main/openapi/docker-hub-authentication-api-api-openapi.yml
- filename: docker-hub-groups-api-openapi.yml
  format: yaml
  label: Docker Hub groups API
  slug: docker-hub-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/docker-hub/refs/heads/main/openapi/docker-hub-groups-api-openapi.yml
- filename: docker-hub-invites-api-openapi.yml
  format: yaml
  label: Docker Hub invites API
  slug: docker-hub-invites-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/docker-hub/refs/heads/main/openapi/docker-hub-invites-api-openapi.yml
- filename: docker-hub-org-access-tokens-api-openapi.yml
  format: yaml
  label: Docker Hub org-access-tokens API
  slug: docker-hub-org-access-tokens-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/docker-hub/refs/heads/main/openapi/docker-hub-org-access-tokens-api-openapi.yml
- filename: docker-hub-org-settings-api-openapi.yml
  format: yaml
  label: Docker Hub org-settings API
  slug: docker-hub-org-settings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/docker-hub/refs/heads/main/openapi/docker-hub-org-settings-api-openapi.yml
- filename: docker-hub-orgs-api-openapi.yml
  format: yaml
  label: Docker Hub orgs API
  slug: docker-hub-orgs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/docker-hub/refs/heads/main/openapi/docker-hub-orgs-api-openapi.yml
- filename: docker-hub-repositories-api-openapi.yml
  format: yaml
  label: Docker Hub repositories API
  slug: docker-hub-repositories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/docker-hub/refs/heads/main/openapi/docker-hub-repositories-api-openapi.yml
- filename: docker-hub-scim-api-openapi.yml
  format: yaml
  label: Docker Hub scim API
  slug: docker-hub-scim-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/docker-hub/refs/heads/main/openapi/docker-hub-scim-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 issue "sectigo.com"
  - 0 iodef "mailto:infra+caa-iodef@docker.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: docker.com
  spf: true
hosts:
- cert_expires: Oct  4 19:28:21 2026 GMT
  host: hub.docker.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan  2 23:59:59 2027 GMT
  host: docs.docker.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Docker Hub Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Docker Hub, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Docker Hub
provider_slug: docker-hub
slug: docker-hub-domain-security
source_filename: docker-hub-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: hub.docker.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 19:28:21 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.docker.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  2 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: docker.com\n  dnssec: false\n  caa:\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"sectigo.com\"\n  - 0 iodef \"mailto:infra+caa-iodef@docker.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/docker-hub/refs/heads/main/security/docker-hub-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Containers
- DevOps
- Docker
- Registry
---
