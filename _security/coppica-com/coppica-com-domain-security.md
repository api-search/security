---
api_specs:
- filename: coppica-com-clients-api-openapi.yml
  format: yaml
  label: Coppica Clients API
  slug: coppica-com-clients-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coppica-com/openapi/coppica-com-clients-api-openapi.yml
- filename: coppica-com-deploy-track-api-openapi.yml
  format: yaml
  label: Coppica Deploy & track API
  slug: coppica-com-deploy-track-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coppica-com/openapi/coppica-com-deploy-track-api-openapi.yml
- filename: coppica-com-generation-api-openapi.yml
  format: yaml
  label: Coppica Generation API
  slug: coppica-com-generation-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coppica-com/openapi/coppica-com-generation-api-openapi.yml
- filename: coppica-com-learning-loop-api-openapi.yml
  format: yaml
  label: Coppica Learning loop API
  slug: coppica-com-learning-loop-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coppica-com/openapi/coppica-com-learning-loop-api-openapi.yml
- filename: coppica-com-reference-api-openapi.yml
  format: yaml
  label: Coppica Reference API
  slug: coppica-com-reference-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coppica-com/openapi/coppica-com-reference-api-openapi.yml
- filename: coppica-com-resources-api-openapi.yml
  format: yaml
  label: Coppica Resources API
  slug: coppica-com-resources-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coppica-com/openapi/coppica-com-resources-api-openapi.yml
- filename: coppica-com-webhooks-api-openapi.yml
  format: yaml
  label: Coppica Webhooks API
  slug: coppica-com-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coppica-com/openapi/coppica-com-webhooks-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 issue "sectigo.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: coppica.com
  spf: true
hosts:
- cert_expires: Jan 28 03:18:56 2027 GMT
  host: coppica.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Coppica Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Coppica, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Coppica
provider_slug: coppica-com
slug: coppica-com-domain-security
source_filename: coppica-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: coppica.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 28 03:18:56 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: coppica.com\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"sectigo.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/coppica-com/security/coppica-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Marketing
- Copywriting
- Generative AI
- Advertising
- Conversion Tracking
- Attribution
- MCP
- AI Agents
---
