---
api_specs:
- filename: distribution-tech-audience-api-openapi.yml
  format: yaml
  label: distribution-tech Audience API
  slug: distribution-tech-audience-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/distribution-tech/openapi/distribution-tech-audience-api-openapi.yml
- filename: distribution-tech-brain-api-openapi.yml
  format: yaml
  label: distribution-tech Brain API
  slug: distribution-tech-brain-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/distribution-tech/openapi/distribution-tech-brain-api-openapi.yml
- filename: distribution-tech-campaigns-api-openapi.yml
  format: yaml
  label: distribution-tech Campaigns API
  slug: distribution-tech-campaigns-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/distribution-tech/openapi/distribution-tech-campaigns-api-openapi.yml
- filename: distribution-tech-creators-api-openapi.yml
  format: yaml
  label: distribution-tech Creators API
  slug: distribution-tech-creators-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/distribution-tech/openapi/distribution-tech-creators-api-openapi.yml
- filename: distribution-tech-evidence-api-openapi.yml
  format: yaml
  label: distribution-tech Evidence API
  slug: distribution-tech-evidence-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/distribution-tech/openapi/distribution-tech-evidence-api-openapi.yml
- filename: distribution-tech-feedback-api-openapi.yml
  format: yaml
  label: distribution-tech Feedback API
  slug: distribution-tech-feedback-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/distribution-tech/openapi/distribution-tech-feedback-api-openapi.yml
- filename: distribution-tech-inventory-api-openapi.yml
  format: yaml
  label: distribution-tech Inventory API
  slug: distribution-tech-inventory-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/distribution-tech/openapi/distribution-tech-inventory-api-openapi.yml
- filename: distribution-tech-plans-api-openapi.yml
  format: yaml
  label: distribution-tech Plans API
  slug: distribution-tech-plans-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/distribution-tech/openapi/distribution-tech-plans-api-openapi.yml
- filename: distribution-tech-results-api-openapi.yml
  format: yaml
  label: distribution-tech Results API
  slug: distribution-tech-results-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/distribution-tech/openapi/distribution-tech-results-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  - 0 iodef "mailto:team@distribution.tech"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: distribution.tech
  spf: true
hosts:
- cert_expires: Jan  4 19:37:04 2027 GMT
  host: distribution.tech
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Distribution Tech Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for distribution-tech, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: distribution-tech
provider_slug: distribution-tech
slug: distribution-tech-domain-security
source_filename: distribution-tech-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-22'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: distribution.tech\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  4 19:37:04 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: distribution.tech\n  dnssec: true\n  caa:\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  - 0 iodef \"mailto:team@distribution.tech\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/distribution-tech/security/distribution-tech-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Distribution
- Marketing
- SaaS
- CreatorEconomy
---
