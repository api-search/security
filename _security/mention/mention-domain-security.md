---
api_specs:
- filename: mention-openapi.yml
  format: yaml
  label: Mention API
  slug: mention-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mention/refs/heads/main/openapi/mention-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: mention.com
  spf: true
hosts:
- cert_expires: Sep 25 18:13:52 2026 GMT
  host: mention.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 13 23:40:21 2026 GMT
  host: api.mention.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Mention Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Mention, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Mention
provider_slug: mention
slug: mention-domain-security
source_filename: mention-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: mention.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 25 18:13:52 2026 GMT\n  hsts: false\n- host: api.mention.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 13 23:40:21 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: mention.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mention/refs/heads/main/security/mention-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Alerts
- Brand Monitoring
- Media Monitoring
- Social Listening
---
