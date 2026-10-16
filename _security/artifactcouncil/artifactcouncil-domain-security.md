---
api_specs:
- filename: artifactcouncil-api-openapi.json
  format: json
  label: Artifact Council API (Solana mainnet) API
  slug: artifact-council-api-solana-mainnet-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/artifactcouncil/refs/heads/main/openapi/_original/artifactcouncil-api-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: artifactcouncil.com
  spf: true
hosts:
- cert_expires: Dec 15 22:03:43 2026 GMT
  host: artifactcouncil.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Artifactcouncil Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Artifact Council, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Artifact Council
provider_slug: artifactcouncil
slug: artifactcouncil-domain-security
source_filename: artifactcouncil-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: artifactcouncil.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 15 22:03:43 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: artifactcouncil.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/artifactcouncil/refs/heads/main/security/artifactcouncil-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Decentralized
- Knowledge
- Solana
- API
---
