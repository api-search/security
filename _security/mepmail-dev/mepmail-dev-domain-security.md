---
api_specs:
- filename: mepmail-dev-account-api-openapi.yml
  format: yaml
  label: MepMail Account API
  slug: mepmail-dev-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mepmail-dev/openapi/mepmail-dev-account-api-openapi.yml
- filename: mepmail-dev-api-keys-api-openapi.yml
  format: yaml
  label: MepMail API keys API
  slug: mepmail-dev-api-keys-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mepmail-dev/openapi/mepmail-dev-api-keys-api-openapi.yml
- filename: mepmail-dev-audiences-api-openapi.yml
  format: yaml
  label: MepMail Audiences API
  slug: mepmail-dev-audiences-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mepmail-dev/openapi/mepmail-dev-audiences-api-openapi.yml
- filename: mepmail-dev-broadcasts-api-openapi.yml
  format: yaml
  label: MepMail Broadcasts API
  slug: mepmail-dev-broadcasts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mepmail-dev/openapi/mepmail-dev-broadcasts-api-openapi.yml
- filename: mepmail-dev-contact-properties-api-openapi.yml
  format: yaml
  label: MepMail Contact properties API
  slug: mepmail-dev-contact-properties-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mepmail-dev/openapi/mepmail-dev-contact-properties-api-openapi.yml
- filename: mepmail-dev-contacts-api-openapi.yml
  format: yaml
  label: MepMail Contacts API
  slug: mepmail-dev-contacts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mepmail-dev/openapi/mepmail-dev-contacts-api-openapi.yml
- filename: mepmail-dev-domains-api-openapi.yml
  format: yaml
  label: MepMail Domains API
  slug: mepmail-dev-domains-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mepmail-dev/openapi/mepmail-dev-domains-api-openapi.yml
- filename: mepmail-dev-emails-api-openapi.yml
  format: yaml
  label: MepMail Emails API
  slug: mepmail-dev-emails-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mepmail-dev/openapi/mepmail-dev-emails-api-openapi.yml
- filename: mepmail-dev-segments-api-openapi.yml
  format: yaml
  label: MepMail Segments API
  slug: mepmail-dev-segments-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mepmail-dev/openapi/mepmail-dev-segments-api-openapi.yml
- filename: mepmail-dev-suppressions-api-openapi.yml
  format: yaml
  label: MepMail Suppressions API
  slug: mepmail-dev-suppressions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mepmail-dev/openapi/mepmail-dev-suppressions-api-openapi.yml
- filename: mepmail-dev-templates-api-openapi.yml
  format: yaml
  label: MepMail Templates API
  slug: mepmail-dev-templates-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mepmail-dev/openapi/mepmail-dev-templates-api-openapi.yml
- filename: mepmail-dev-topics-api-openapi.yml
  format: yaml
  label: MepMail Topics API
  slug: mepmail-dev-topics-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mepmail-dev/openapi/mepmail-dev-topics-api-openapi.yml
- filename: mepmail-dev-webhooks-api-openapi.yml
  format: yaml
  label: MepMail Webhooks API
  slug: mepmail-dev-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mepmail-dev/openapi/mepmail-dev-webhooks-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "ssl.com"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: mepmail.dev
  spf: true
hosts:
- cert_expires: Jan  8 14:31:39 2027 GMT
  host: mepmail.dev
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: MepMail Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for MepMail, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: MepMail
provider_slug: mepmail-dev
slug: mepmail-dev-domain-security
source_filename: mepmail-dev-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: mepmail.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  8 14:31:39 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: mepmail.dev\n  dnssec: true\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/mepmail-dev/security/mepmail-dev-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Email
- Services
- Communications
- Developers
---
