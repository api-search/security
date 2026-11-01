---
api_specs:
- filename: gaianet-ai-openapi-generated.yml
  format: yaml
  label: GaiaNet API
  slug: gaianet-ai-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gaianet-ai/openapi/_ae-authored/gaianet-ai-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: gaianet.ai
  spf: true
hosts:
- cert_expires: Feb 20 23:59:59 2027 GMT
  host: gaianet.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Gaianet Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for GaiaNet, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: GaiaNet
provider_slug: gaianet-ai
slug: gaianet-ai-domain-security
source_filename: gaianet-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: gaianet.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 20 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: gaianet.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/gaianet-ai/security/gaianet-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Decentralization
- Artificial Intelligence
- Privacy
- Security
- Governance
- Networks
---
