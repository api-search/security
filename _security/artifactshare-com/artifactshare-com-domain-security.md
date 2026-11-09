---
api_specs:
- filename: artifactshare-com-cli-api-openapi.yml
  format: yaml
  label: Artifact Share Cli API
  slug: artifactshare-com-cli-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/artifactshare-com/openapi/artifactshare-com-cli-api-openapi.yml
- filename: artifactshare-com-mcp-api-openapi.yml
  format: yaml
  label: Artifact Share MCP API
  slug: artifactshare-com-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/artifactshare-com/openapi/artifactshare-com-mcp-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: artifactshare.com
  spf: true
hosts:
- cert_expires: Jan 17 01:47:29 2027 GMT
  host: artifactshare.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Artifactshare Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Artifact Share, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Artifact Share
provider_slug: artifactshare-com
slug: artifactshare-com-domain-security
source_filename: artifactshare-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-01'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: artifactshare.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 17 01:47:29 2027 GMT\n  hsts: false\ndomains:\n- domain: artifactshare.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/artifactshare-com/security/artifactshare-com-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- File Sharing
- HTML
- Markdown
- AI Integration
- Developer Tools
---
