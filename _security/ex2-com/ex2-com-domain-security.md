---
api_specs:
- filename: ex2-com-compare-api-openapi.yml
  format: yaml
  label: ex2-com Compare API
  slug: ex2-com-compare-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ex2-com/openapi/ex2-com-compare-api-openapi.yml
- filename: ex2-com-domains-api-openapi.yml
  format: yaml
  label: ex2-com Domains API
  slug: ex2-com-domains-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ex2-com/openapi/ex2-com-domains-api-openapi.yml
- filename: ex2-com-ex2-catalogue-api-api-openapi.yml
  format: yaml
  label: ex2-com Ex2 Catalogue API
  slug: ex2-com-ex2-catalogue-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ex2-com/openapi/ex2-com-ex2-catalogue-api-api-openapi.yml
- filename: ex2-com-migration-api-openapi.yml
  format: yaml
  label: ex2-com Migration API
  slug: ex2-com-migration-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ex2-com/openapi/ex2-com-migration-api-openapi.yml
- filename: ex2-com-plans-api-openapi.yml
  format: yaml
  label: ex2-com Plans API
  slug: ex2-com-plans-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ex2-com/openapi/ex2-com-plans-api-openapi.yml
- filename: ex2-com-status-api-openapi.yml
  format: yaml
  label: ex2-com Status API
  slug: ex2-com-status-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ex2-com/openapi/ex2-com-status-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "ssl.com"
  - 0 issuewild "comodoca.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: ex2.com
  spf: true
hosts:
- cert_expires: Dec 12 23:59:59 2026 GMT
  host: ex2.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Ex2 Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ex2-com, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: ex2-com
provider_slug: ex2-com
slug: ex2-com-domain-security
source_filename: ex2-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ex2.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 12 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: ex2.com\n  dnssec: true\n  caa:\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"comodoca.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/ex2-com/security/ex2-com-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Hosting
- Sustainability
- WebHosting
- Quebec
- GreenTech
---
