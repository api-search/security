---
api_specs:
- filename: tabfleet-com-health-api-openapi.yml
  format: yaml
  label: Tabfleet Health API
  slug: tabfleet-com-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tabfleet-com/openapi/tabfleet-com-health-api-openapi.yml
- filename: tabfleet-com-sessions-api-openapi.yml
  format: yaml
  label: Tabfleet Sessions API
  slug: tabfleet-com-sessions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tabfleet-com/openapi/tabfleet-com-sessions-api-openapi.yml
- filename: tabfleet-com-usage-api-openapi.yml
  format: yaml
  label: Tabfleet Usage API
  slug: tabfleet-com-usage-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tabfleet-com/openapi/tabfleet-com-usage-api-openapi.yml
- filename: tabfleet-com-viewer-settings-api-openapi.yml
  format: yaml
  label: Tabfleet Viewer Settings API
  slug: tabfleet-com-viewer-settings-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tabfleet-com/openapi/tabfleet-com-viewer-settings-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dns_aid:
    agents: []
    checked: '2026-11-25'
    index:
    - alpn:
      - h2
      target: tabfleet.com
    published: true
  dnssec: true
  domain: tabfleet.com
  spf: true
hosts:
- cert_expires: Feb  8 18:37:56 2027 GMT
  host: tabfleet.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Tabfleet Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Tabfleet, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Tabfleet
provider_slug: tabfleet-com
slug: tabfleet-com-domain-security
source_filename: tabfleet-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-25'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: tabfleet.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  8 18:37:56 2027 GMT\n  hsts: false\ndomains:\n- domain: tabfleet.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n  dns_aid:\n    checked: '2026-11-25'\n    published: true\n    index:\n    - target: tabfleet.com\n      alpn:\n      - h2\n    agents: []\n"
source_yaml_url: https://artifacts.apis.io/tabfleet-com/security/tabfleet-com-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Cloud
- Browser
- AI
- Infrastructure
- MCP
---
