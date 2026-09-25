---
api_specs:
- filename: caamtech-mcp-api-openapi.yml
  format: yaml
  label: CaaMTech MCP API
  slug: caamtech-mcp-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/caamtech/refs/heads/main/openapi/caamtech-mcp-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: caam.tech
  spf: true
hosts:
- cert_expires: Nov  6 06:02:39 2026 GMT
  host: caam.tech
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Caamtech Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for CaaMTech, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: CaaMTech
provider_slug: caamtech
slug: caamtech-domain-security
source_filename: caamtech-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-08'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: caam.tech\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  6 06:02:39 2026 GMT\n  hsts: false\ndomains:\n- domain: caam.tech\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/caamtech/refs/heads/main/security/caamtech-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Pharmaceuticals
- Life Sciences
- Drug Discovery
- Biotechnology
- Chemistry
- Mental Health
- Research
- Psychedelics
- WordPress
---
