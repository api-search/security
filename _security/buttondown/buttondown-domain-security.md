---
api_specs:
- filename: buttondown-openapi.yml
  format: yaml
  label: Buttondown API
  slug: buttondown-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/buttondown/refs/heads/main/openapi/buttondown-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: buttondown.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: buttondown.email
  spf: true
hosts:
- cert_expires: Aug 22 00:20:38 2026 GMT
  host: buttondown.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 21 00:07:46 2026 GMT
  host: docs.buttondown.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  8 01:53:40 2026 GMT
  host: api.buttondown.email
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Buttondown Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Buttondown, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Buttondown
provider_slug: buttondown
slug: buttondown-domain-security
source_filename: buttondown-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: buttondown.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 22 00:20:38 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.buttondown.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 21 00:07:46 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.buttondown.email\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  8 01:53:40 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: buttondown.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: buttondown.email\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/buttondown/refs/heads/main/security/buttondown-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Analytics
- Automations
- Email
- Markdown
- Newsletters
- Paid Subscriptions
- SaaS
- Subscribers
---
