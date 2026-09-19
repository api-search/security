---
api_specs:
- filename: quaker-houghton-tribe-events-v1-openapi-original.json
  format: json
  label: Quaker Houghton Events API
  slug: quaker-houghton-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/quaker-houghton/refs/heads/main/openapi/_original/quaker-houghton-tribe-events-v1-openapi-original.json
- filename: quaker-houghton-tec-v1-openapi-original.json
  format: json
  label: Quaker Houghton TEC v1 Events API
  slug: quaker-houghton-tec-v1-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/quaker-houghton/refs/heads/main/openapi/_original/quaker-houghton-tec-v1-openapi-original.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: quakerhoughton.com
  spf: true
hosts:
- cert_expires: Dec 22 23:59:59 2026 GMT
  host: home.quakerhoughton.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Quaker Houghton Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Quaker Houghton, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Quaker Houghton
provider_slug: quaker-houghton
slug: quaker-houghton-domain-security
source_filename: quaker-houghton-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: home.quakerhoughton.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 22 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: quakerhoughton.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/quaker-houghton/refs/heads/main/security/quaker-houghton-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Industrial Fluids
- Chemicals
- Manufacturing
- Metalworking
- Lubricants
- Event
- MCP
---
