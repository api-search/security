---
api_specs:
- filename: podman-artifacts-api-openapi.yml
  format: yaml
  label: Podman artifacts API
  slug: podman-artifacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/podman/refs/heads/main/openapi/podman-artifacts-api-openapi.yml
- filename: podman-containers-api-openapi.yml
  format: yaml
  label: Podman containers API
  slug: podman-containers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/podman/refs/heads/main/openapi/podman-containers-api-openapi.yml
- filename: podman-containers-compat-api-openapi.yml
  format: yaml
  label: Podman containers (compat) API
  slug: podman-containers-compat-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/podman/refs/heads/main/openapi/podman-containers-compat-api-openapi.yml
- filename: podman-exec-api-openapi.yml
  format: yaml
  label: Podman exec API
  slug: podman-exec-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/podman/refs/heads/main/openapi/podman-exec-api-openapi.yml
- filename: podman-exec-compat-api-openapi.yml
  format: yaml
  label: Podman exec (compat) API
  slug: podman-exec-compat-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/podman/refs/heads/main/openapi/podman-exec-compat-api-openapi.yml
- filename: podman-images-api-openapi.yml
  format: yaml
  label: Podman images API
  slug: podman-images-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/podman/refs/heads/main/openapi/podman-images-api-openapi.yml
- filename: podman-images-compat-api-openapi.yml
  format: yaml
  label: Podman images (compat) API
  slug: podman-images-compat-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/podman/refs/heads/main/openapi/podman-images-compat-api-openapi.yml
- filename: podman-manifests-api-openapi.yml
  format: yaml
  label: Podman manifests API
  slug: podman-manifests-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/podman/refs/heads/main/openapi/podman-manifests-api-openapi.yml
- filename: podman-networks-api-openapi.yml
  format: yaml
  label: Podman networks API
  slug: podman-networks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/podman/refs/heads/main/openapi/podman-networks-api-openapi.yml
- filename: podman-networks-compat-api-openapi.yml
  format: yaml
  label: Podman networks (compat) API
  slug: podman-networks-compat-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/podman/refs/heads/main/openapi/podman-networks-compat-api-openapi.yml
- filename: podman-pods-api-openapi.yml
  format: yaml
  label: Podman pods API
  slug: podman-pods-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/podman/refs/heads/main/openapi/podman-pods-api-openapi.yml
- filename: podman-quadlets-api-openapi.yml
  format: yaml
  label: Podman quadlets API
  slug: podman-quadlets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/podman/refs/heads/main/openapi/podman-quadlets-api-openapi.yml
- filename: podman-secrets-api-openapi.yml
  format: yaml
  label: Podman secrets API
  slug: podman-secrets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/podman/refs/heads/main/openapi/podman-secrets-api-openapi.yml
- filename: podman-secrets-compat-api-openapi.yml
  format: yaml
  label: Podman secrets (compat) API
  slug: podman-secrets-compat-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/podman/refs/heads/main/openapi/podman-secrets-compat-api-openapi.yml
- filename: podman-system-api-openapi.yml
  format: yaml
  label: Podman system API
  slug: podman-system-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/podman/refs/heads/main/openapi/podman-system-api-openapi.yml
- filename: podman-system-compat-api-openapi.yml
  format: yaml
  label: Podman system (compat) API
  slug: podman-system-compat-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/podman/refs/heads/main/openapi/podman-system-compat-api-openapi.yml
- filename: podman-volumes-api-openapi.yml
  format: yaml
  label: Podman volumes API
  slug: podman-volumes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/podman/refs/heads/main/openapi/podman-volumes-api-openapi.yml
- filename: podman-volumes-compat-api-openapi.yml
  format: yaml
  label: Podman volumes (compat) API
  slug: podman-volumes-compat-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/podman/refs/heads/main/openapi/podman-volumes-compat-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: podman.io
  spf: true
hosts:
- cert_expires: Sep 19 22:09:50 2026 GMT
  host: podman.io
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  4 01:59:03 2026 GMT
  host: docs.podman.io
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Podman Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Podman, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Podman
provider_slug: podman
slug: podman-domain-security
source_filename: podman-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: podman.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 19 22:09:50 2026 GMT\n  hsts: false\n- host: docs.podman.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 01:59:03 2026 GMT\n  hsts: false\ndomains:\n- domain: podman.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/podman/refs/heads/main/security/podman-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Cloud-Native
- Containers
- DevOps
- OCI
- Open-Source
---
