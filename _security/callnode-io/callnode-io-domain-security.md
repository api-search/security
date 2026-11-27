---
api_specs:
- filename: callnode-io-call-records-api-openapi.yml
  format: yaml
  label: CallNode Call Records API
  slug: callnode-io-call-records-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/callnode-io/openapi/callnode-io-call-records-api-openapi.yml
- filename: callnode-io-email-api-openapi.yml
  format: yaml
  label: CallNode Email API
  slug: callnode-io-email-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/callnode-io/openapi/callnode-io-email-api-openapi.yml
- filename: callnode-io-faxes-api-openapi.yml
  format: yaml
  label: CallNode Faxes API
  slug: callnode-io-faxes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/callnode-io/openapi/callnode-io-faxes-api-openapi.yml
- filename: callnode-io-messaging-api-openapi.yml
  format: yaml
  label: CallNode Messaging API
  slug: callnode-io-messaging-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/callnode-io/openapi/callnode-io-messaging-api-openapi.yml
- filename: callnode-io-outbound-calls-api-openapi.yml
  format: yaml
  label: CallNode Outbound Calls API
  slug: callnode-io-outbound-calls-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/callnode-io/openapi/callnode-io-outbound-calls-api-openapi.yml
- filename: callnode-io-phone-numbers-api-openapi.yml
  format: yaml
  label: CallNode Phone Numbers API
  slug: callnode-io-phone-numbers-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/callnode-io/openapi/callnode-io-phone-numbers-api-openapi.yml
- filename: callnode-io-sip-trunks-api-openapi.yml
  format: yaml
  label: CallNode SIP Trunks API
  slug: callnode-io-sip-trunks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/callnode-io/openapi/callnode-io-sip-trunks-api-openapi.yml
- filename: callnode-io-wholesale-api-openapi.yml
  format: yaml
  label: CallNode Wholesale API
  slug: callnode-io-wholesale-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/callnode-io/openapi/callnode-io-wholesale-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: callnode.io
  spf: true
hosts:
- cert_expires: Dec 25 17:43:50 2026 GMT
  host: callnode.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: CallNode Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for CallNode, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: CallNode
provider_slug: callnode-io
slug: callnode-io-domain-security
source_filename: callnode-io-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-03'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: callnode.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 25 17:43:50 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: callnode.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/callnode-io/security/callnode-io-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Voice AI
- Telephony
- Phone Numbers
- SMS
- Webhook
- SIP Trunking
- AI Agents
- Communications
---
