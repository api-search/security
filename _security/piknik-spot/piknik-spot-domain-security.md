---
api_specs:
- filename: piknik-spot-openapi.yml
  format: yaml
  label: Piknik.Spot REST API
  slug: piknikspot-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/piknik-spot/refs/heads/main/openapi/piknik-spot-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: piknik.spot
  spf: true
hosts:
- cert_expires: Nov  1 06:22:38 2026 GMT
  host: piknik.spot
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Piknik Spot Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Piknik.Spot, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Piknik.Spot
provider_slug: piknik-spot
slug: piknik-spot-domain-security
source_filename: piknik-spot-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: piknik.spot\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  1 06:22:38 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: piknik.spot\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/piknik-spot/refs/heads/main/security/piknik-spot-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Local Food
- Agriculture
- Farmers Markets
- Marketplace
- Event
- Job
- Recipes
- Geolocation
- Community
- Food Systems
- MCP
- A2A
- Agent-Native
- Ontario
- Canada
---
