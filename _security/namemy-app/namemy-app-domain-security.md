---
api_specs:
- filename: namemy-app-brand-conflict-api-openapi.yml
  format: yaml
  label: Namemy Brand Conflict API
  slug: namemy-app-brand-conflict-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/namemy-app/openapi/namemy-app-brand-conflict-api-openapi.yml
- filename: namemy-app-brand-kits-api-openapi.yml
  format: yaml
  label: Namemy Brand Kits API
  slug: namemy-app-brand-kits-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/namemy-app/openapi/namemy-app-brand-kits-api-openapi.yml
- filename: namemy-app-domains-api-openapi.yml
  format: yaml
  label: Namemy Domains API
  slug: namemy-app-domains-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/namemy-app/openapi/namemy-app-domains-api-openapi.yml
- filename: namemy-app-keys-api-openapi.yml
  format: yaml
  label: Namemy Keys API
  slug: namemy-app-keys-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/namemy-app/openapi/namemy-app-keys-api-openapi.yml
- filename: namemy-app-landing-pages-api-openapi.yml
  format: yaml
  label: Namemy Landing Pages API
  slug: namemy-app-landing-pages-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/namemy-app/openapi/namemy-app-landing-pages-api-openapi.yml
- filename: namemy-app-legal-api-openapi.yml
  format: yaml
  label: Namemy Legal API
  slug: namemy-app-legal-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/namemy-app/openapi/namemy-app-legal-api-openapi.yml
- filename: namemy-app-logos-api-openapi.yml
  format: yaml
  label: Namemy Logos API
  slug: namemy-app-logos-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/namemy-app/openapi/namemy-app-logos-api-openapi.yml
- filename: namemy-app-names-api-openapi.yml
  format: yaml
  label: Namemy Names API
  slug: namemy-app-names-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/namemy-app/openapi/namemy-app-names-api-openapi.yml
- filename: namemy-app-public-api-openapi.yml
  format: yaml
  label: Namemy Public API
  slug: namemy-app-public-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/namemy-app/openapi/namemy-app-public-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: namemy.app
  spf: true
hosts:
- cert_expires: Jan 17 16:11:37 2027 GMT
  host: namemy.app
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Namemy Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Namemy, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Namemy
provider_slug: namemy-app
slug: namemy-app-domain-security
source_filename: namemy-app-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: namemy.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 17 16:11:37 2027 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: namemy.app\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/namemy-app/security/namemy-app-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Artificial Intelligence
- Naming
- Domain
- Software-as-a-Service
---
