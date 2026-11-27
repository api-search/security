---
api_specs:
- filename: mailbox-bot-api-openapi.json
  format: json
  label: mailbox.bot API API
  slug: mailbox-bot-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mailbox-bot/openapi/_original/mailbox-bot-api-openapi.json
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 issue "sectigo.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: mailbox.bot
  spf: true
hosts:
- cert_expires: Jan 12 08:07:02 2027 GMT
  host: mailbox.bot
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Mailbox.bot Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Mailbox.bot, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Mailbox.bot
provider_slug: mailbox-bot
slug: mailbox-bot-domain-security
source_filename: mailbox-bot-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: mailbox.bot\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 12 08:07:02 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: mailbox.bot\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"sectigo.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/mailbox-bot/security/mailbox-bot-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Artificial Intelligence
- Mail
- Automation
- Postal
---
