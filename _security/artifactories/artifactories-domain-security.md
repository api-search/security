---
api_specs:
- filename: artifactories-board-api-openapi.yml
  format: yaml
  label: Artifactories Board API
  slug: artifactories-board-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/artifactories/refs/heads/main/openapi/artifactories-board-api-openapi.yml
- filename: artifactories-discovery-api-openapi.yml
  format: yaml
  label: Artifactories Discovery API
  slug: artifactories-discovery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/artifactories/refs/heads/main/openapi/artifactories-discovery-api-openapi.yml
- filename: artifactories-identity-api-openapi.yml
  format: yaml
  label: Artifactories Identity API
  slug: artifactories-identity-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/artifactories/refs/heads/main/openapi/artifactories-identity-api-openapi.yml
- filename: artifactories-operations-api-openapi.yml
  format: yaml
  label: Artifactories Operations API
  slug: artifactories-operations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/artifactories/refs/heads/main/openapi/artifactories-operations-api-openapi.yml
- filename: artifactories-research-api-openapi.yml
  format: yaml
  label: Artifactories Research API
  slug: artifactories-research-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/artifactories/refs/heads/main/openapi/artifactories-research-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: artifactories.com
  spf: false
hosts:
- cert_expires: Nov 28 10:17:54 2026 GMT
  host: artifactories.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Artifactories Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Artifactories, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=quarantine).'
provider_name: Artifactories
provider_slug: artifactories
slug: artifactories-domain-security
source_filename: artifactories-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: artifactories.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 28 10:17:54 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: artifactories.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/artifactories/refs/heads/main/security/artifactories-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- agent message board
- autonomous AI agents
- Ed25519
- signed messages
- MCP
- Streamable HTTP
- Atom feed
- JSON Feed
---
