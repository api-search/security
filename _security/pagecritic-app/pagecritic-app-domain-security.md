---
api_specs:
- filename: pagecritic-app-audit-api-openapi.yml
  format: yaml
  label: PageCritic Audit API
  slug: pagecritic-app-audit-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/pagecritic-app/openapi/pagecritic-app-audit-api-openapi.yml
- filename: pagecritic-app-credits-api-openapi.yml
  format: yaml
  label: PageCritic Credits API
  slug: pagecritic-app-credits-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/pagecritic-app/openapi/pagecritic-app-credits-api-openapi.yml
- filename: pagecritic-app-keys-api-openapi.yml
  format: yaml
  label: PageCritic Keys API
  slug: pagecritic-app-keys-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/pagecritic-app/openapi/pagecritic-app-keys-api-openapi.yml
- filename: pagecritic-app-readiness-api-openapi.yml
  format: yaml
  label: PageCritic Readiness API
  slug: pagecritic-app-readiness-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/pagecritic-app/openapi/pagecritic-app-readiness-api-openapi.yml
- filename: pagecritic-app-recheck-api-openapi.yml
  format: yaml
  label: PageCritic Recheck API
  slug: pagecritic-app-recheck-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/pagecritic-app/openapi/pagecritic-app-recheck-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: pagecritic.app
  spf: true
hosts:
- cert_expires: Jan 16 00:37:35 2027 GMT
  host: pagecritic.app
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: PageCritic Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for PageCritic, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: PageCritic
provider_slug: pagecritic-app
slug: pagecritic-app-domain-security
source_filename: pagecritic-app-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: pagecritic.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 16 00:37:35 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: pagecritic.app\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/pagecritic-app/security/pagecritic-app-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Artificial Intelligence
- Landing Pages
- Audit
- Software-as-a-Service
---
