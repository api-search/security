---
api_specs:
- filename: interos-groups-api-openapi.yml
  format: yaml
  label: Interos Groups API
  slug: interos-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/interos/refs/heads/main/openapi/interos-groups-api-openapi.yml
- filename: interos-health-api-openapi.yml
  format: yaml
  label: Interos health API
  slug: interos-health-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/interos/refs/heads/main/openapi/interos-health-api-openapi.yml
- filename: interos-organizations-api-openapi.yml
  format: yaml
  label: Interos Organizations API
  slug: interos-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/interos/refs/heads/main/openapi/interos-organizations-api-openapi.yml
- filename: interos-relationships-api-openapi.yml
  format: yaml
  label: Interos Relationships API
  slug: interos-relationships-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/interos/refs/heads/main/openapi/interos-relationships-api-openapi.yml
- filename: interos-watchtower-api-openapi.yml
  format: yaml
  label: Interos Watchtower API
  slug: interos-watchtower-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/interos/refs/heads/main/openapi/interos-watchtower-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: interos.ai
  spf: true
hosts:
- cert_expires: Oct  7 16:41:24 2026 GMT
  host: www.interos.ai
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Interos Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Interos, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Interos
provider_slug: interos
slug: interos-domain-security
source_filename: interos-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.interos.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  7 16:41:24 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: interos.ai\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/interos/refs/heads/main/security/interos-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Enterprise
- Supply Chain
- Risk Management
- Supplier Risk
- Third-Party Risk
- Artificial Intelligence
---
