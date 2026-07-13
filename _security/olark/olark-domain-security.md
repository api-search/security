---
api_specs:
- filename: olark-openapi.yml
  format: yaml
  label: Olark JavaScript API
  slug: javascript-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/olark/refs/heads/main/openapi/olark-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: olark.com
  spf: true
hosts:
- cert_expires: Aug 13 06:29:58 2026 GMT
  host: www.olark.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Olark Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Olark, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Olark
provider_slug: olark
slug: olark-domain-security
source_filename: olark-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.olark.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 13 06:29:58 2026 GMT\n  hsts: false\ndomains:\n- domain: olark.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/olark/refs/heads/main/security/olark-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Live Chat
- Customer Support
- Chatbots
- Customer Engagement
- Messaging
- Accessibility
---
