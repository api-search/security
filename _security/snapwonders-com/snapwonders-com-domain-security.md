---
api_specs:
- filename: snapwonders-com-analyse-api-openapi.yml
  format: yaml
  label: snapwonders-com Analyse API
  slug: snapwonders-com-analyse-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/snapwonders-com/openapi/snapwonders-com-analyse-api-openapi.yml
- filename: snapwonders-com-convert-api-openapi.yml
  format: yaml
  label: snapwonders-com Convert API
  slug: snapwonders-com-convert-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/snapwonders-com/openapi/snapwonders-com-convert-api-openapi.yml
- filename: snapwonders-com-hide-api-openapi.yml
  format: yaml
  label: snapwonders-com Hide API
  slug: snapwonders-com-hide-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/snapwonders-com/openapi/snapwonders-com-hide-api-openapi.yml
- filename: snapwonders-com-mcp-api-openapi.yml
  format: yaml
  label: snapwonders-com MCP API
  slug: snapwonders-com-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/snapwonders-com/openapi/snapwonders-com-mcp-api-openapi.yml
- filename: snapwonders-com-media-upload-direct-api-openapi.yml
  format: yaml
  label: snapwonders-com Media Upload - Direct API
  slug: snapwonders-com-media-upload-direct-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/snapwonders-com/openapi/snapwonders-com-media-upload-direct-api-openapi.yml
- filename: snapwonders-com-media-upload-tus-resumable-api-openapi.yml
  format: yaml
  label: snapwonders-com Media Upload - TUS Resumable API
  slug: snapwonders-com-media-upload-tus-resumable-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/snapwonders-com/openapi/snapwonders-com-media-upload-tus-resumable-api-openapi.yml
- filename: snapwonders-com-reveal-api-openapi.yml
  format: yaml
  label: snapwonders-com Reveal API
  slug: snapwonders-com-reveal-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/snapwonders-com/openapi/snapwonders-com-reveal-api-openapi.yml
- filename: snapwonders-com-status-api-openapi.yml
  format: yaml
  label: snapwonders-com Status API
  slug: snapwonders-com-status-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/snapwonders-com/openapi/snapwonders-com-status-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "snapwonders.com"
  - 0 issue "ssl.com"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: snapwonders.com
  spf: true
hosts:
- cert_expires: Jan 20 18:03:35 2027 GMT
  host: snapwonders.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Snapwonders Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for snapwonders-com, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: snapwonders-com
provider_slug: snapwonders-com
slug: snapwonders-com-domain-security
source_filename: snapwonders-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: snapwonders.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 20 18:03:35 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: snapwonders.com\n  dnssec: true\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"snapwonders.com\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/snapwonders-com/security/snapwonders-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Forensics
- Steganography
- MediaConversion
- Privacy
- Open Source
---
