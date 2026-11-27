---
api_specs:
- filename: agenthost-eu-openapi-generated.yml
  format: yaml
  label: agenthost API
  slug: agenthost-eu-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agenthost-eu/openapi/_ae-authored/agenthost-eu-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: agenthost.eu
  spf: true
hosts:
- cert_expires: Jan 13 18:26:21 2027 GMT
  host: agenthost.eu
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: agenthost Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for agenthost, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: agenthost
provider_slug: agenthost-eu
slug: agenthost-eu-domain-security
source_filename: agenthost-eu-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: agenthost.eu\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 13 18:26:21 2027 GMT\n  hsts: false\ndomains:\n- domain: agenthost.eu\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/agenthost-eu/security/agenthost-eu-domain-security.yml
summary_line: TLSv1.3
tags:
- Web Hosting
- Artificial Intelligence
- MCP
- Cloud
- EU
---
