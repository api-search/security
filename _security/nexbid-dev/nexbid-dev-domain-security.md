---
api_specs:
- filename: nexbid-dev-agent-api-openapi.yml
  format: yaml
  label: nexbid-dev Agent API
  slug: nexbid-dev-agent-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nexbid-dev/openapi/nexbid-dev-agent-api-openapi.yml
- filename: nexbid-dev-attribution-api-openapi.yml
  format: yaml
  label: nexbid-dev Attribution API
  slug: nexbid-dev-attribution-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nexbid-dev/openapi/nexbid-dev-attribution-api-openapi.yml
- filename: nexbid-dev-discovery-api-openapi.yml
  format: yaml
  label: nexbid-dev Discovery API
  slug: nexbid-dev-discovery-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nexbid-dev/openapi/nexbid-dev-discovery-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: nexbid.dev
  spf: true
hosts:
- cert_expires: Jan 25 13:48:20 2027 GMT
  host: nexbid.dev
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Nexbid Dev Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for nexbid-dev, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: nexbid-dev
provider_slug: nexbid-dev
slug: nexbid-dev-domain-security
source_filename: nexbid-dev-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: nexbid.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 25 13:48:20 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: nexbid.dev\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/nexbid-dev/security/nexbid-dev-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- AI
- Commerce
- Advertising
- Switzerland
- OpenSource
---
