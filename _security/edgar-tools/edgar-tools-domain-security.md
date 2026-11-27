---
api_specs:
- filename: edgar-tools-openapi-generated.yml
  format: yaml
  label: edgar.tools API
  slug: edgar-tools-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/edgar-tools/openapi/_ae-authored/edgar-tools-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: edgar.tools
  spf: true
hosts:
- cert_expires: Jan 11 03:32:12 2027 GMT
  host: edgar.tools
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: edgar.tools Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for edgar.tools, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: edgar.tools
provider_slug: edgar-tools
slug: edgar-tools-domain-security
source_filename: edgar-tools-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-06'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: edgar.tools\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 11 03:32:12 2027 GMT\n  hsts: false\ndomains:\n- domain: edgar.tools\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/edgar-tools/security/edgar-tools-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Finance
- Artificial Intelligence
- SEC
- Data
- MCP
---
