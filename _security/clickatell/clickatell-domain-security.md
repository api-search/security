---
api_specs:
- filename: clickatell-chat-2-pay-api-api-openapi.yml
  format: yaml
  label: Clickatell Chat 2 Pay API
  slug: clickatell-chat-2-pay-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clickatell/refs/heads/main/openapi/clickatell-chat-2-pay-api-api-openapi.yml
- filename: clickatell-chat-2-pay-api-client-callbacks-api-openapi.yml
  format: yaml
  label: Clickatell Chat 2 Pay API Client Callbacks API
  slug: clickatell-chat-2-pay-api-client-callbacks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clickatell/refs/heads/main/openapi/clickatell-chat-2-pay-api-client-callbacks-api-openapi.yml
- filename: clickatell-external-link-callback-api-openapi.yml
  format: yaml
  label: Clickatell External Link Callback API
  slug: clickatell-external-link-callback-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clickatell/refs/heads/main/openapi/clickatell-external-link-callback-api-openapi.yml
- filename: clickatell-one-api-api-openapi.yml
  format: yaml
  label: Clickatell One API
  slug: clickatell-one-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clickatell/refs/heads/main/openapi/clickatell-one-api-api-openapi.yml
- filename: clickatell-one-api-client-callbacks-api-openapi.yml
  format: yaml
  label: Clickatell One API Client Callbacks API
  slug: clickatell-one-api-client-callbacks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clickatell/refs/heads/main/openapi/clickatell-one-api-client-callbacks-api-openapi.yml
- filename: clickatell-sms-api-api-openapi.yml
  format: yaml
  label: Clickatell SMS API
  slug: clickatell-sms-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clickatell/refs/heads/main/openapi/clickatell-sms-api-api-openapi.yml
- filename: clickatell-sms-client-callbacks-api-openapi.yml
  format: yaml
  label: Clickatell SMS Client Callbacks API
  slug: clickatell-sms-client-callbacks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clickatell/refs/heads/main/openapi/clickatell-sms-client-callbacks-api-openapi.yml
- filename: clickatell-wait-for-callback-api-openapi.yml
  format: yaml
  label: Clickatell Wait for Callback API
  slug: clickatell-wait-for-callback-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clickatell/refs/heads/main/openapi/clickatell-wait-for-callback-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "amazon.com"
  - 0 issue "godaddy.com"
  - 0 issue "digicert.com"
  - 0 issue "pki.goog"
  - 0 issue "globalsign.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: clickatell.com
  spf: true
hosts:
- cert_expires: Jan 30 23:59:59 2027 GMT
  host: www.clickatell.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Clickatell Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Clickatell, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Clickatell
provider_slug: clickatell
slug: clickatell-domain-security
source_filename: clickatell-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.clickatell.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 30 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: clickatell.com\n  dnssec: false\n  caa:\n  - 0 issue \"amazon.com\"\n  - 0 issue \"godaddy.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"globalsign.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/clickatell/refs/heads/main/security/clickatell-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- SMS
- WhatsApp
- Messaging
- CPaaS
- Chat Commerce
- Payments
---
