---
api_specs:
- filename: hex-pm-api-keys-api-openapi.yml
  format: yaml
  label: Hex.pm API Keys API
  slug: hex-pm-api-keys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hex-pm/refs/heads/main/openapi/hex-pm-api-keys-api-openapi.yml
- filename: hex-pm-authentication-api-openapi.yml
  format: yaml
  label: Hex.pm Authentication API
  slug: hex-pm-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hex-pm/refs/heads/main/openapi/hex-pm-authentication-api-openapi.yml
- filename: hex-pm-documentation-api-openapi.yml
  format: yaml
  label: Hex.pm Documentation API
  slug: hex-pm-documentation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hex-pm/refs/heads/main/openapi/hex-pm-documentation-api-openapi.yml
- filename: hex-pm-index-api-openapi.yml
  format: yaml
  label: Hex.pm Index API
  slug: hex-pm-index-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hex-pm/refs/heads/main/openapi/hex-pm-index-api-openapi.yml
- filename: hex-pm-oauth-api-openapi.yml
  format: yaml
  label: Hex.pm OAuth API
  slug: hex-pm-oauth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hex-pm/refs/heads/main/openapi/hex-pm-oauth-api-openapi.yml
- filename: hex-pm-organizations-api-openapi.yml
  format: yaml
  label: Hex.pm Organizations API
  slug: hex-pm-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hex-pm/refs/heads/main/openapi/hex-pm-organizations-api-openapi.yml
- filename: hex-pm-package-owners-api-openapi.yml
  format: yaml
  label: Hex.pm Package Owners API
  slug: hex-pm-package-owners-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hex-pm/refs/heads/main/openapi/hex-pm-package-owners-api-openapi.yml
- filename: hex-pm-packages-api-openapi.yml
  format: yaml
  label: Hex.pm Packages API
  slug: hex-pm-packages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hex-pm/refs/heads/main/openapi/hex-pm-packages-api-openapi.yml
- filename: hex-pm-releases-api-openapi.yml
  format: yaml
  label: Hex.pm Releases API
  slug: hex-pm-releases-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hex-pm/refs/heads/main/openapi/hex-pm-releases-api-openapi.yml
- filename: hex-pm-repositories-api-openapi.yml
  format: yaml
  label: Hex.pm Repositories API
  slug: hex-pm-repositories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hex-pm/refs/heads/main/openapi/hex-pm-repositories-api-openapi.yml
- filename: hex-pm-users-api-openapi.yml
  format: yaml
  label: Hex.pm Users API
  slug: hex-pm-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hex-pm/refs/heads/main/openapi/hex-pm-users-api-openapi.yml
- filename: hex-pm-utilities-api-openapi.yml
  format: yaml
  label: Hex.pm Utilities API
  slug: hex-pm-utilities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hex-pm/refs/heads/main/openapi/hex-pm-utilities-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: hex.pm
  spf: true
hosts:
- cert_expires: Aug 29 00:20:27 2026 GMT
  host: hex.pm
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Hex Pm Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Hex.pm, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Hex.pm
provider_slug: hex-pm
slug: hex-pm-domain-security
source_filename: hex-pm-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: hex.pm\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 29 00:20:27 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: hex.pm\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hex-pm/refs/heads/main/security/hex-pm-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Package Registry
- Erlang
- Elixir
- Gleam
- BEAM
- Open Source
- Package Manager
---
