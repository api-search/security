---
api_specs:
- filename: forward-email-account-api-openapi.yml
  format: yaml
  label: Forward Email Account API
  slug: forward-email-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/forward-email/openapi/forward-email-account-api-openapi.yml
- filename: forward-email-aliases-api-openapi.yml
  format: yaml
  label: Forward Email Aliases API
  slug: forward-email-aliases-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/forward-email/openapi/forward-email-aliases-api-openapi.yml
- filename: forward-email-calendar-events-api-openapi.yml
  format: yaml
  label: Forward Email Calendar Events API
  slug: forward-email-calendar-events-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/forward-email/openapi/forward-email-calendar-events-api-openapi.yml
- filename: forward-email-calendars-api-openapi.yml
  format: yaml
  label: Forward Email Calendars API
  slug: forward-email-calendars-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/forward-email/openapi/forward-email-calendars-api-openapi.yml
- filename: forward-email-contacts-api-openapi.yml
  format: yaml
  label: Forward Email Contacts API
  slug: forward-email-contacts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/forward-email/openapi/forward-email-contacts-api-openapi.yml
- filename: forward-email-domains-api-openapi.yml
  format: yaml
  label: Forward Email Domains API
  slug: forward-email-domains-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/forward-email/openapi/forward-email-domains-api-openapi.yml
- filename: forward-email-emails-api-openapi.yml
  format: yaml
  label: Forward Email Emails API
  slug: forward-email-emails-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/forward-email/openapi/forward-email-emails-api-openapi.yml
- filename: forward-email-encrypt-api-openapi.yml
  format: yaml
  label: Forward Email Encrypt API
  slug: forward-email-encrypt-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/forward-email/openapi/forward-email-encrypt-api-openapi.yml
- filename: forward-email-folders-api-openapi.yml
  format: yaml
  label: Forward Email Folders API
  slug: forward-email-folders-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/forward-email/openapi/forward-email-folders-api-openapi.yml
- filename: forward-email-invites-api-openapi.yml
  format: yaml
  label: Forward Email Invites API
  slug: forward-email-invites-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/forward-email/openapi/forward-email-invites-api-openapi.yml
- filename: forward-email-logs-api-openapi.yml
  format: yaml
  label: Forward Email Logs API
  slug: forward-email-logs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/forward-email/openapi/forward-email-logs-api-openapi.yml
- filename: forward-email-members-api-openapi.yml
  format: yaml
  label: Forward Email Members API
  slug: forward-email-members-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/forward-email/openapi/forward-email-members-api-openapi.yml
- filename: forward-email-messages-api-openapi.yml
  format: yaml
  label: Forward Email Messages API
  slug: forward-email-messages-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/forward-email/openapi/forward-email-messages-api-openapi.yml
- filename: forward-email-push-tokens-api-openapi.yml
  format: yaml
  label: Forward Email Push Tokens API
  slug: forward-email-push-tokens-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/forward-email/openapi/forward-email-push-tokens-api-openapi.yml
- filename: forward-email-sieve-scripts-api-openapi.yml
  format: yaml
  label: Forward Email Sieve Scripts API
  slug: forward-email-sieve-scripts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/forward-email/openapi/forward-email-sieve-scripts-api-openapi.yml
- filename: forward-email-websockets-api-openapi.yml
  format: yaml
  label: Forward Email WebSockets API
  slug: forward-email-websockets-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/forward-email/openapi/forward-email-websockets-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "sectigo.com; cansignhttpexchanges=yes "
  - 0 issue "ssl.com"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: forwardemail.net
  spf: true
hosts:
- cert_expires: Jan 20 23:59:59 2027 GMT
  host: forwardemail.net
  hsts: true
  hsts_max_age: 31557600
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Forward Email Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Forward Email, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Forward Email
provider_slug: forward-email
slug: forward-email-domain-security
source_filename: forward-email-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: forwardemail.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 20 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31557600\ndomains:\n- domain: forwardemail.net\n  dnssec: true\n  caa:\n  - 0 issue \"sectigo.com; cansignhttpexchanges=yes \"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/forward-email/security/forward-email-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Email Forwarding
- Email Hosting
- Open Source
- API
- Secure Email
---
