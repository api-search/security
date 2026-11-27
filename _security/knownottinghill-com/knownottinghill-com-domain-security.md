---
api_specs:
- filename: knownottinghill-com-agent-api-openapi.yml
  format: yaml
  label: KnowNottingHill Agent API
  slug: knownottinghill-com-agent-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/knownottinghill-com/openapi/knownottinghill-com-agent-api-openapi.yml
- filename: knownottinghill-com-places-api-openapi.yml
  format: yaml
  label: KnowNottingHill Places API
  slug: knownottinghill-com-places-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/knownottinghill-com/openapi/knownottinghill-com-places-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: knownottinghill.com
  spf: true
hosts:
- cert_expires: Jan 16 11:35:21 2027 GMT
  host: knownottinghill.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: KnowNottingHill Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for KnowNottingHill, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: KnowNottingHill
provider_slug: knownottinghill-com
slug: knownottinghill-com-domain-security
source_filename: knownottinghill-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: knownottinghill.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 16 11:35:21 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: knownottinghill.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/knownottinghill-com/security/knownottinghill-com-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Community
- guide
- London
- Notting Hill
- Neighborhood
---
