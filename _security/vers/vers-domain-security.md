---
api_specs:
- filename: vers-commit-tags-api-openapi.yml
  format: yaml
  label: Vers commit_tags API
  slug: vers-commit-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vers/refs/heads/main/openapi/vers-commit-tags-api-openapi.yml
- filename: vers-commits-api-openapi.yml
  format: yaml
  label: Vers commits API
  slug: vers-commits-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vers/refs/heads/main/openapi/vers-commits-api-openapi.yml
- filename: vers-deploy-api-openapi.yml
  format: yaml
  label: Vers deploy API
  slug: vers-deploy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vers/refs/heads/main/openapi/vers-deploy-api-openapi.yml
- filename: vers-domains-api-openapi.yml
  format: yaml
  label: Vers domains API
  slug: vers-domains-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vers/refs/heads/main/openapi/vers-domains-api-openapi.yml
- filename: vers-env-vars-api-openapi.yml
  format: yaml
  label: Vers env_vars API
  slug: vers-env-vars-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vers/refs/heads/main/openapi/vers-env-vars-api-openapi.yml
- filename: vers-images-api-openapi.yml
  format: yaml
  label: Vers images API
  slug: vers-images-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vers/refs/heads/main/openapi/vers-images-api-openapi.yml
- filename: vers-keys-api-openapi.yml
  format: yaml
  label: Vers keys API
  slug: vers-keys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vers/refs/heads/main/openapi/vers-keys-api-openapi.yml
- filename: vers-public-repositories-api-openapi.yml
  format: yaml
  label: Vers public_repositories API
  slug: vers-public-repositories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vers/refs/heads/main/openapi/vers-public-repositories-api-openapi.yml
- filename: vers-repositories-api-openapi.yml
  format: yaml
  label: Vers repositories API
  slug: vers-repositories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vers/refs/heads/main/openapi/vers-repositories-api-openapi.yml
- filename: vers-system-api-openapi.yml
  format: yaml
  label: Vers System API
  slug: vers-system-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vers/refs/heads/main/openapi/vers-system-api-openapi.yml
- filename: vers-vm-api-openapi.yml
  format: yaml
  label: Vers vm API
  slug: vers-vm-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vers/refs/heads/main/openapi/vers-vm-api-openapi.yml
- filename: vers-vms-api-openapi.yml
  format: yaml
  label: Vers vms API
  slug: vers-vms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vers/refs/heads/main/openapi/vers-vms-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: vers.sh
  spf: true
hosts:
- cert_expires: Sep 15 16:26:08 2026 GMT
  host: vers.sh
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 15 16:19:43 2026 GMT
  host: docs.vers.sh
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 18 21:07:28 2026 GMT
  host: api.vers.sh
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Vers Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Vers, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Vers
provider_slug: vers
slug: vers-domain-security
source_filename: vers-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: vers.sh\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 16:26:08 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.vers.sh\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 16:19:43 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.vers.sh\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 18 21:07:28 2026 GMT\n  hsts: false\ndomains:\n- domain: vers.sh\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vers/refs/heads/main/security/vers-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Compute
- Virtualization
- MicroVM
- Orchestration
- Infrastructure
- AI Agents
- Developer Tools
- Sandbox
- CI/CD
---
