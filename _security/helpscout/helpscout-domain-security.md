---
api_specs:
- filename: helpscout-openapi.yml
  format: yaml
  label: Help Scout Conversations API
  slug: helpscout-conversations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/helpscout/refs/heads/main/openapi/helpscout-openapi.yml
- filename: helpscout-webhooks-asyncapi.yml
  format: yaml
  label: Help Scout Webhooks API
  slug: helpscout-webhooks-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/helpscout/refs/heads/main/asyncapi/helpscout-webhooks-asyncapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: helpscout.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: helpscout.net
  spf: true
hosts:
- cert_expires: Sep 26 22:11:27 2026 GMT
  host: www.helpscout.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 23 11:33:38 2026 GMT
  host: api.helpscout.net
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Helpscout Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Help Scout, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Help Scout
provider_slug: helpscout
slug: helpscout-domain-security
source_filename: helpscout-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.helpscout.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 26 22:11:27 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.helpscout.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 23 11:33:38 2026 GMT\n  hsts: null\ndomains:\n- domain: helpscout.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: helpscout.net\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/helpscout/refs/heads/main/security/helpscout-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Customer Support
- Help Desk
- Email
- Live Chat
- Knowledge Base
- SaaS
---
