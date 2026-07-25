---
api_specs:
- filename: itch-io-auth-api-openapi.yml
  format: yaml
  label: Itch.io Auth API
  slug: itch-io-auth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/itch-io/refs/heads/main/openapi/itch-io-auth-api-openapi.yml
- filename: itch-io-builds-api-openapi.yml
  format: yaml
  label: Itch.io Builds API
  slug: itch-io-builds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/itch-io/refs/heads/main/openapi/itch-io-builds-api-openapi.yml
- filename: itch-io-bundles-api-openapi.yml
  format: yaml
  label: Itch.io Bundles API
  slug: itch-io-bundles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/itch-io/refs/heads/main/openapi/itch-io-bundles-api-openapi.yml
- filename: itch-io-collections-api-openapi.yml
  format: yaml
  label: Itch.io Collections API
  slug: itch-io-collections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/itch-io/refs/heads/main/openapi/itch-io-collections-api-openapi.yml
- filename: itch-io-downloads-api-openapi.yml
  format: yaml
  label: Itch.io Downloads API
  slug: itch-io-downloads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/itch-io/refs/heads/main/openapi/itch-io-downloads-api-openapi.yml
- filename: itch-io-games-api-openapi.yml
  format: yaml
  label: Itch.io Games API
  slug: itch-io-games-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/itch-io/refs/heads/main/openapi/itch-io-games-api-openapi.yml
- filename: itch-io-profile-api-openapi.yml
  format: yaml
  label: Itch.io Profile API
  slug: itch-io-profile-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/itch-io/refs/heads/main/openapi/itch-io-profile-api-openapi.yml
- filename: itch-io-search-api-openapi.yml
  format: yaml
  label: Itch.io Search API
  slug: itch-io-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/itch-io/refs/heads/main/openapi/itch-io-search-api-openapi.yml
- filename: itch-io-uploads-api-openapi.yml
  format: yaml
  label: Itch.io Uploads API
  slug: itch-io-uploads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/itch-io/refs/heads/main/openapi/itch-io-uploads-api-openapi.yml
- filename: itch-io-users-api-openapi.yml
  format: yaml
  label: Itch.io Users API
  slug: itch-io-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/itch-io/refs/heads/main/openapi/itch-io-users-api-openapi.yml
- filename: itch-io-wharf-api-openapi.yml
  format: yaml
  label: Itch.io Wharf API
  slug: itch-io-wharf-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/itch-io/refs/heads/main/openapi/itch-io-wharf-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: itch.io
  spf: true
hosts:
- cert_expires: Sep 20 13:15:02 2026 GMT
  host: itch.io
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 20 13:15:02 2026 GMT
  host: api.itch.io
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Itch Io Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Itch.io, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Itch.io
provider_slug: itch-io
slug: itch-io-domain-security
source_filename: itch-io-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: itch.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 20 13:15:02 2026 GMT\n  hsts: false\n- host: api.itch.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 20 13:15:02 2026 GMT\n  hsts: null\ndomains:\n- domain: itch.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/itch-io/refs/heads/main/security/itch-io-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Games
- Indie Games
- Game Distribution
- Game Marketplace
- Developers
---
