---
api_specs:
- filename: basecite-com-admin-api-openapi.yml
  format: yaml
  label: BaseCite Admin API
  slug: basecite-com-admin-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/basecite-com/openapi/basecite-com-admin-api-openapi.yml
- filename: basecite-com-ai-api-openapi.yml
  format: yaml
  label: BaseCite AI API
  slug: basecite-com-ai-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/basecite-com/openapi/basecite-com-ai-api-openapi.yml
- filename: basecite-com-oauth-api-openapi.yml
  format: yaml
  label: BaseCite OAuth API
  slug: basecite-com-oauth-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/basecite-com/openapi/basecite-com-oauth-api-openapi.yml
- filename: basecite-com-organizations-api-openapi.yml
  format: yaml
  label: BaseCite Organizations API
  slug: basecite-com-organizations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/basecite-com/openapi/basecite-com-organizations-api-openapi.yml
- filename: basecite-com-portal-api-openapi.yml
  format: yaml
  label: BaseCite Portal API
  slug: basecite-com-portal-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/basecite-com/openapi/basecite-com-portal-api-openapi.yml
- filename: basecite-com-sandbox-api-openapi.yml
  format: yaml
  label: BaseCite Sandbox API
  slug: basecite-com-sandbox-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/basecite-com/openapi/basecite-com-sandbox-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: basecite.com
  spf: true
hosts:
- cert_expires: Jan 12 12:35:07 2027 GMT
  host: basecite.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: BaseCite Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for BaseCite, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: BaseCite
provider_slug: basecite-com
slug: basecite-com-domain-security
source_filename: basecite-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: basecite.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 12 12:35:07 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: basecite.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/basecite-com/security/basecite-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Artificial Intelligence
- Evidence
- Platform
- Privacy
---
