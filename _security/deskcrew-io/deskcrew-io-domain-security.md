---
api_specs:
- filename: deskcrew-io-app-api-openapi.yml
  format: yaml
  label: DeskCrew App API
  slug: deskcrew-io-app-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/deskcrew-io/openapi/deskcrew-io-app-api-openapi.yml
- filename: deskcrew-io-billing-api-openapi.yml
  format: yaml
  label: DeskCrew Billing API
  slug: deskcrew-io-billing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/deskcrew-io/openapi/deskcrew-io-billing-api-openapi.yml
- filename: deskcrew-io-bounties-api-openapi.yml
  format: yaml
  label: DeskCrew Bounties API
  slug: deskcrew-io-bounties-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/deskcrew-io/openapi/deskcrew-io-bounties-api-openapi.yml
- filename: deskcrew-io-changelog-api-openapi.yml
  format: yaml
  label: DeskCrew Changelog API
  slug: deskcrew-io-changelog-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/deskcrew-io/openapi/deskcrew-io-changelog-api-openapi.yml
- filename: deskcrew-io-changes-api-openapi.yml
  format: yaml
  label: DeskCrew Changes API
  slug: deskcrew-io-changes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/deskcrew-io/openapi/deskcrew-io-changes-api-openapi.yml
- filename: deskcrew-io-customers-api-openapi.yml
  format: yaml
  label: DeskCrew Customers API
  slug: deskcrew-io-customers-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/deskcrew-io/openapi/deskcrew-io-customers-api-openapi.yml
- filename: deskcrew-io-devices-api-openapi.yml
  format: yaml
  label: DeskCrew Devices API
  slug: deskcrew-io-devices-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/deskcrew-io/openapi/deskcrew-io-devices-api-openapi.yml
- filename: deskcrew-io-errors-api-openapi.yml
  format: yaml
  label: DeskCrew Errors API
  slug: deskcrew-io-errors-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/deskcrew-io/openapi/deskcrew-io-errors-api-openapi.yml
- filename: deskcrew-io-issues-api-openapi.yml
  format: yaml
  label: DeskCrew Issues API
  slug: deskcrew-io-issues-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/deskcrew-io/openapi/deskcrew-io-issues-api-openapi.yml
- filename: deskcrew-io-kb-api-openapi.yml
  format: yaml
  label: DeskCrew Kb API
  slug: deskcrew-io-kb-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/deskcrew-io/openapi/deskcrew-io-kb-api-openapi.yml
- filename: deskcrew-io-me-api-openapi.yml
  format: yaml
  label: DeskCrew Me API
  slug: deskcrew-io-me-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/deskcrew-io/openapi/deskcrew-io-me-api-openapi.yml
- filename: deskcrew-io-paid-agent-tools-api-openapi.yml
  format: yaml
  label: DeskCrew Paid agent tools API
  slug: deskcrew-io-paid-agent-tools-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/deskcrew-io/openapi/deskcrew-io-paid-agent-tools-api-openapi.yml
- filename: deskcrew-io-tickets-api-openapi.yml
  format: yaml
  label: DeskCrew Tickets API
  slug: deskcrew-io-tickets-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/deskcrew-io/openapi/deskcrew-io-tickets-api-openapi.yml
- filename: deskcrew-io-webhooks-api-openapi.yml
  format: yaml
  label: DeskCrew Webhooks API
  slug: deskcrew-io-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/deskcrew-io/openapi/deskcrew-io-webhooks-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  - 0 iodef "mailto:hello@deskcrew.io"
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: deskcrew.io
  spf: true
hosts:
- cert_expires: Jan 11 16:02:29 2027 GMT
  host: deskcrew.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: DeskCrew Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for DeskCrew, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: DeskCrew
provider_slug: deskcrew-io
slug: deskcrew-io-domain-security
source_filename: deskcrew-io-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: deskcrew.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 11 16:02:29 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: deskcrew.io\n  dnssec: true\n  caa:\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  - 0 iodef \"mailto:hello@deskcrew.io\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/deskcrew-io/security/deskcrew-io-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Help Desk
- AI Agents
- MCP
- Support
---
