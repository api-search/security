---
api_specs:
- filename: local-infusion-wp-v2-api-openapi.yml
  format: yaml
  label: Local Infusion WordPress Content API
  slug: local-infusion-wp-v2-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/local-infusion/refs/heads/main/openapi/local-infusion-wp-v2-api-openapi.yml
- filename: local-infusion-mcp-api-openapi.yml
  format: yaml
  label: Local Infusion MCP API
  slug: local-infusion-mcp-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/local-infusion/refs/heads/main/openapi/local-infusion-mcp-api-openapi.yml
- filename: local-infusion-wp-abilities-v1-api-openapi.yml
  format: yaml
  label: Local Infusion WordPress Abilities API
  slug: local-infusion-wp-abilities-v1-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/local-infusion/refs/heads/main/openapi/local-infusion-wp-abilities-v1-api-openapi.yml
- filename: local-infusion-root-api-openapi.yml
  format: yaml
  label: Local Infusion WordPress Root API
  slug: local-infusion-root-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/local-infusion/refs/heads/main/openapi/local-infusion-root-api-openapi.yml
- filename: local-infusion-oembed-1-0-api-openapi.yml
  format: yaml
  label: Local Infusion oEmbed API
  slug: local-infusion-oembed-1-0-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/local-infusion/refs/heads/main/openapi/local-infusion-oembed-1-0-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: mylocalinfusion.com
  spf: true
hosts:
- cert_expires: Oct 22 07:00:11 2026 GMT
  host: mylocalinfusion.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Local Infusion Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Local Infusion, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Local Infusion
provider_slug: local-infusion
slug: local-infusion-domain-security
source_filename: local-infusion-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-25'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: mylocalinfusion.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 22 07:00:11 2026 GMT\n  hsts: false\ndomains:\n- domain: mylocalinfusion.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/local-infusion/refs/heads/main/security/local-infusion-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Healthcare
- Health Services
- Infusion Therapy
- Specialty Pharmacy
- Ambulatory Care
- Patient Services
- Autoimmune
- Chronic Care
- MCP
- WordPress
---
