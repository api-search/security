---
api_specs:
- filename: majr-app-audit-api-openapi.yml
  format: yaml
  label: majr-app Audit API
  slug: majr-app-audit-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/majr-app/openapi/majr-app-audit-api-openapi.yml
- filename: majr-app-discovery-api-openapi.yml
  format: yaml
  label: majr-app Discovery API
  slug: majr-app-discovery-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/majr-app/openapi/majr-app-discovery-api-openapi.yml
- filename: majr-app-drafting-api-openapi.yml
  format: yaml
  label: majr-app Drafting API
  slug: majr-app-drafting-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/majr-app/openapi/majr-app-drafting-api-openapi.yml
- filename: majr-app-encode-api-openapi.yml
  format: yaml
  label: majr-app Encode API
  slug: majr-app-encode-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/majr-app/openapi/majr-app-encode-api-openapi.yml
- filename: majr-app-generation-api-openapi.yml
  format: yaml
  label: majr-app Generation API
  slug: majr-app-generation-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/majr-app/openapi/majr-app-generation-api-openapi.yml
- filename: majr-app-healthz-api-openapi.yml
  format: yaml
  label: majr-app Healthz API
  slug: majr-app-healthz-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/majr-app/openapi/majr-app-healthz-api-openapi.yml
- filename: majr-app-jobs-api-openapi.yml
  format: yaml
  label: majr-app Jobs API
  slug: majr-app-jobs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/majr-app/openapi/majr-app-jobs-api-openapi.yml
- filename: majr-app-uploads-api-openapi.yml
  format: yaml
  label: majr-app Uploads API
  slug: majr-app-uploads-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/majr-app/openapi/majr-app-uploads-api-openapi.yml
- filename: majr-app-usage-api-openapi.yml
  format: yaml
  label: majr-app Usage API
  slug: majr-app-usage-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/majr-app/openapi/majr-app-usage-api-openapi.yml
- filename: majr-app-voice-api-openapi.yml
  format: yaml
  label: majr-app Voice API
  slug: majr-app-voice-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/majr-app/openapi/majr-app-voice-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: majr.app
  spf: true
hosts:
- cert_expires: Jan 10 23:52:57 2027 GMT
  host: majr.app
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Majr App Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for majr-app, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: majr-app
provider_slug: majr-app
slug: majr-app-domain-security
source_filename: majr-app-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: majr.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 10 23:52:57 2027 GMT\n  hsts: false\ndomains:\n- domain: majr.app\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/majr-app/security/majr-app-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- AI
- Media
- SEO
- Encoding
- Agent Services
---
