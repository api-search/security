---
api_specs:
- filename: cosmicjs-com-blocks-api-openapi.yml
  format: yaml
  label: Cosmic Blocks API
  slug: cosmicjs-com-blocks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cosmicjs-com/openapi/cosmicjs-com-blocks-api-openapi.yml
- filename: cosmicjs-com-media-api-openapi.yml
  format: yaml
  label: Cosmic Media API
  slug: cosmicjs-com-media-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cosmicjs-com/openapi/cosmicjs-com-media-api-openapi.yml
- filename: cosmicjs-com-object-revisions-api-openapi.yml
  format: yaml
  label: Cosmic Object revisions API
  slug: cosmicjs-com-object-revisions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cosmicjs-com/openapi/cosmicjs-com-object-revisions-api-openapi.yml
- filename: cosmicjs-com-object-types-api-openapi.yml
  format: yaml
  label: Cosmic Object types API
  slug: cosmicjs-com-object-types-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cosmicjs-com/openapi/cosmicjs-com-object-types-api-openapi.yml
- filename: cosmicjs-com-objects-api-openapi.yml
  format: yaml
  label: Cosmic Objects API
  slug: cosmicjs-com-objects-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cosmicjs-com/openapi/cosmicjs-com-objects-api-openapi.yml
- filename: cosmicjs-com-status-api-openapi.yml
  format: yaml
  label: Cosmic Status API
  slug: cosmicjs-com-status-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cosmicjs-com/openapi/cosmicjs-com-status-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: cosmicjs.com
  spf: true
hosts:
- cert_expires: Dec 13 12:32:58 2026 GMT
  host: www.cosmicjs.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Cosmic Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cosmic, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Cosmic
provider_slug: cosmicjs-com
slug: cosmicjs-com-domain-security
source_filename: cosmicjs-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.cosmicjs.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 13 12:32:58 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: cosmicjs.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/cosmicjs-com/security/cosmicjs-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Headless CMS
- Content Management
- content-api
- AI Agents
- MCP
- Webhook
- JAMstack
---
