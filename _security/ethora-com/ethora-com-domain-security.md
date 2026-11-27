---
api_specs:
- filename: ethora-com-agents-api-openapi.yml
  format: yaml
  label: Ethora Agents API
  slug: ethora-com-agents-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ethora-com/openapi/ethora-com-agents-api-openapi.yml
- filename: ethora-com-ai-widget-api-openapi.yml
  format: yaml
  label: Ethora AI Widget API
  slug: ethora-com-ai-widget-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ethora-com/openapi/ethora-com-ai-widget-api-openapi.yml
- filename: ethora-com-apps-api-openapi.yml
  format: yaml
  label: Ethora Apps API
  slug: ethora-com-apps-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ethora-com/openapi/ethora-com-apps-api-openapi.yml
- filename: ethora-com-auth-api-openapi.yml
  format: yaml
  label: Ethora Auth API
  slug: ethora-com-auth-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ethora-com/openapi/ethora-com-auth-api-openapi.yml
- filename: ethora-com-chats-api-openapi.yml
  format: yaml
  label: Ethora Chats API
  slug: ethora-com-chats-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ethora-com/openapi/ethora-com-chats-api-openapi.yml
- filename: ethora-com-files-api-openapi.yml
  format: yaml
  label: Ethora Files API
  slug: ethora-com-files-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ethora-com/openapi/ethora-com-files-api-openapi.yml
- filename: ethora-com-push-api-openapi.yml
  format: yaml
  label: Ethora Push API
  slug: ethora-com-push-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ethora-com/openapi/ethora-com-push-api-openapi.yml
- filename: ethora-com-sharelinks-api-openapi.yml
  format: yaml
  label: Ethora Sharelinks API
  slug: ethora-com-sharelinks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ethora-com/openapi/ethora-com-sharelinks-api-openapi.yml
- filename: ethora-com-users-api-openapi.yml
  format: yaml
  label: Ethora Users API
  slug: ethora-com-users-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ethora-com/openapi/ethora-com-users-api-openapi.yml
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
  dmarc_policy: none
  dnssec: false
  domain: ethora.com
  spf: true
hosts:
- cert_expires: Feb  1 03:08:41 2027 GMT
  host: ethora.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Ethora Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Ethora, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Ethora
provider_slug: ethora-com
slug: ethora-com-domain-security
source_filename: ethora-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-07'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ethora.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  1 03:08:41 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: ethora.com\n  dnssec: false\n  caa:\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"comodoca.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/ethora-com/security/ethora-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Chat
- Artificial Intelligence
- SDK
- Low-Code
- Messaging
---
