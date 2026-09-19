---
api_specs:
- filename: globant-catalog-api-openapi.yml
  format: yaml
  label: Globant Catalog API
  slug: globant-catalog-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/globant/refs/heads/main/openapi/globant-catalog-api-openapi.yml
- filename: globant-health-api-openapi.yml
  format: yaml
  label: Globant Health API
  slug: globant-health-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/globant/refs/heads/main/openapi/globant-health-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: globant.com
  spf: true
hosts:
- cert_expires: Nov 23 07:36:39 2026 GMT
  host: www.globant.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- host: developer.globant.com
  https: false
- cert_expires: Oct 14 15:41:53 2026 GMT
  host: api.globant.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Globant Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Globant, probed live across 3 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Globant
provider_slug: globant
slug: globant-domain-security
source_filename: globant-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-14'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.globant.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 23 07:36:39 2026 GMT\n  hsts: null\n- host: developer.globant.com\n  https: false\n- host: api.globant.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 14 15:41:53 2026 GMT\n  hsts: null\ndomains:\n- domain: globant.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/globant/refs/heads/main/security/globant-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Software
- Digital Transformation
- Artificial Intelligence
- Agents
- MCP
- Consulting
- Enterprise
---
