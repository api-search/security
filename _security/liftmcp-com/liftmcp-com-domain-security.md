---
api_specs:
- filename: liftmcp-com-openapi-generated.yml
  format: yaml
  label: LiftMCP API
  slug: liftmcp-com-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/liftmcp-com/openapi/_ae-authored/liftmcp-com-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: liftmcp.com
  spf: true
hosts:
- cert_expires: Apr 14 23:59:59 2027 GMT
  host: liftmcp.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: LiftMCP Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for LiftMCP, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: LiftMCP
provider_slug: liftmcp-com
slug: liftmcp-com-domain-security
source_filename: liftmcp-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-15'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: liftmcp.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Apr 14 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: liftmcp.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/liftmcp-com/security/liftmcp-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Artificial Intelligence
- Platform
- MCP
- Web
- Integration
---
