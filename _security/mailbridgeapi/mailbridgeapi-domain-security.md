---
api_specs:
- filename: mailbridgeapi-activity-api-openapi.yml
  format: yaml
  label: MailBridgeAPI Activity API
  slug: mailbridgeapi-activity-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mailbridgeapi/openapi/mailbridgeapi-activity-api-openapi.yml
- filename: mailbridgeapi-compliance-api-openapi.yml
  format: yaml
  label: MailBridgeAPI Compliance API
  slug: mailbridgeapi-compliance-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mailbridgeapi/openapi/mailbridgeapi-compliance-api-openapi.yml
- filename: mailbridgeapi-mailbox-api-openapi.yml
  format: yaml
  label: MailBridgeAPI Mailbox API
  slug: mailbridgeapi-mailbox-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mailbridgeapi/openapi/mailbridgeapi-mailbox-api-openapi.yml
- filename: mailbridgeapi-receiving-api-openapi.yml
  format: yaml
  label: MailBridgeAPI Receiving API
  slug: mailbridgeapi-receiving-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mailbridgeapi/openapi/mailbridgeapi-receiving-api-openapi.yml
- filename: mailbridgeapi-sending-api-openapi.yml
  format: yaml
  label: MailBridgeAPI Sending API
  slug: mailbridgeapi-sending-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mailbridgeapi/openapi/mailbridgeapi-sending-api-openapi.yml
- filename: mailbridgeapi-service-api-openapi.yml
  format: yaml
  label: MailBridgeAPI Service API
  slug: mailbridgeapi-service-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mailbridgeapi/openapi/mailbridgeapi-service-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: mailbridgeapi.com
  spf: true
hosts:
- cert_expires: Jan 14 19:38:08 2027 GMT
  host: mailbridgeapi.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Mailbridgeapi Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for MailBridgeAPI, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: MailBridgeAPI
provider_slug: mailbridgeapi
slug: mailbridgeapi-domain-security
source_filename: mailbridgeapi-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: mailbridgeapi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 14 19:38:08 2027 GMT\n  hsts: false\ndomains:\n- domain: mailbridgeapi.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/mailbridgeapi/security/mailbridgeapi-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Email API
- SMTP
- IMAP
- mailbox integration
- Developer Tools
- mailbox monitoring
---
