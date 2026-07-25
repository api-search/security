---
api_specs:
- filename: self-id-commits-api-openapi.yml
  format: yaml
  label: Self.ID Commits API
  slug: self-id-commits-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/self-id/refs/heads/main/openapi/self-id-commits-api-openapi.yml
- filename: self-id-multiqueries-api-openapi.yml
  format: yaml
  label: Self.ID Multiqueries API
  slug: self-id-multiqueries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/self-id/refs/heads/main/openapi/self-id-multiqueries-api-openapi.yml
- filename: self-id-node-api-openapi.yml
  format: yaml
  label: Self.ID Node API
  slug: self-id-node-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/self-id/refs/heads/main/openapi/self-id-node-api-openapi.yml
- filename: self-id-pins-api-openapi.yml
  format: yaml
  label: Self.ID Pins API
  slug: self-id-pins-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/self-id/refs/heads/main/openapi/self-id-pins-api-openapi.yml
- filename: self-id-streams-api-openapi.yml
  format: yaml
  label: Self.ID Streams API
  slug: self-id-streams-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/self-id/refs/heads/main/openapi/self-id-streams-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: ceramic.network
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: 3boxlabs.com
  spf: false
hosts:
- cert_expires: Sep 16 20:45:30 2026 GMT
  host: developers.ceramic.network
  hsts: false
  https: true
  tls_version: TLSv1.3
- host: gateway.ceramic.network
  https: false
- host: ceramic-clay.3boxlabs.com
  https: false
kind: domain-security
layout: security
method: probed
name: Self Id Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Self.ID, probed live across 3 host(s) and 2 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Self.ID
provider_slug: self-id
slug: self-id-domain-security
source_filename: self-id-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developers.ceramic.network\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 16 20:45:30 2026 GMT\n  hsts: false\n- host: gateway.ceramic.network\n  https: false\n- host: ceramic-clay.3boxlabs.com\n  https: false\ndomains:\n- domain: ceramic.network\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n- domain: 3boxlabs.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/self-id/refs/heads/main/security/self-id-domain-security.yml
summary_line: TLSv1.3
tags:
- Decentralized Identity
- DID
- Ceramic
- Self-Sovereign Identity
- Web3
- Verifiable Credentials
- Blockchain
---
