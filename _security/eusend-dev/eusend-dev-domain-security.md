---
api_specs:
- filename: eusend-dev-api-keys-api-openapi.yml
  format: yaml
  label: eusend-dev API keys API
  slug: eusend-dev-api-keys-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/eusend-dev/openapi/eusend-dev-api-keys-api-openapi.yml
- filename: eusend-dev-audiences-api-openapi.yml
  format: yaml
  label: eusend-dev Audiences API
  slug: eusend-dev-audiences-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/eusend-dev/openapi/eusend-dev-audiences-api-openapi.yml
- filename: eusend-dev-broadcasts-api-openapi.yml
  format: yaml
  label: eusend-dev Broadcasts API
  slug: eusend-dev-broadcasts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/eusend-dev/openapi/eusend-dev-broadcasts-api-openapi.yml
- filename: eusend-dev-contact-properties-api-openapi.yml
  format: yaml
  label: eusend-dev Contact properties API
  slug: eusend-dev-contact-properties-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/eusend-dev/openapi/eusend-dev-contact-properties-api-openapi.yml
- filename: eusend-dev-contacts-api-openapi.yml
  format: yaml
  label: eusend-dev Contacts API
  slug: eusend-dev-contacts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/eusend-dev/openapi/eusend-dev-contacts-api-openapi.yml
- filename: eusend-dev-domains-api-openapi.yml
  format: yaml
  label: eusend-dev Domains API
  slug: eusend-dev-domains-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/eusend-dev/openapi/eusend-dev-domains-api-openapi.yml
- filename: eusend-dev-emails-api-openapi.yml
  format: yaml
  label: eusend-dev Emails API
  slug: eusend-dev-emails-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/eusend-dev/openapi/eusend-dev-emails-api-openapi.yml
- filename: eusend-dev-suppressions-api-openapi.yml
  format: yaml
  label: eusend-dev Suppressions API
  slug: eusend-dev-suppressions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/eusend-dev/openapi/eusend-dev-suppressions-api-openapi.yml
- filename: eusend-dev-system-api-openapi.yml
  format: yaml
  label: eusend-dev System API
  slug: eusend-dev-system-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/eusend-dev/openapi/eusend-dev-system-api-openapi.yml
- filename: eusend-dev-templates-api-openapi.yml
  format: yaml
  label: eusend-dev Templates API
  slug: eusend-dev-templates-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/eusend-dev/openapi/eusend-dev-templates-api-openapi.yml
- filename: eusend-dev-topics-api-openapi.yml
  format: yaml
  label: eusend-dev Topics API
  slug: eusend-dev-topics-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/eusend-dev/openapi/eusend-dev-topics-api-openapi.yml
- filename: eusend-dev-webhooks-api-openapi.yml
  format: yaml
  label: eusend-dev Webhooks API
  slug: eusend-dev-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/eusend-dev/openapi/eusend-dev-webhooks-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: eusend.dev
  spf: true
hosts:
- cert_expires: Jan  5 11:22:42 2027 GMT
  host: eusend.dev
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Eusend Dev Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for eusend-dev, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: eusend-dev
provider_slug: eusend-dev
slug: eusend-dev-domain-security
source_filename: eusend-dev-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: eusend.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  5 11:22:42 2027 GMT\n  hsts: false\ndomains:\n- domain: eusend.dev\n  dnssec: true\n  caa:\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/eusend-dev/security/eusend-dev-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Email
- Transactional
- Marketing
- EU
- GDPR
---
