---
api_specs:
- filename: openapi.v2.json
  format: json
  label: MagicBell REST API v2
  slug: rest-api-v2
  spec_type: OpenAPI
  url: https://public.magicbell.com/specs/openapi.v2.json
- filename: 2sAYdhLAjv
  format: yaml
  label: MagicBell REST API v1
  slug: rest-api-v1
  spec_type: Postman
  url: https://documenter.getpostman.com/view/2269098/2sAYdhLAjv
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: magicbell.com
  spf: false
hosts:
- cert_expires: Sep  2 01:23:11 2026 GMT
  host: www.magicbell.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  2 01:23:11 2026 GMT
  host: api.magicbell.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Magicbell Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for MagicBell, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: MagicBell
provider_slug: magicbell
slug: magicbell-domain-security
source_filename: magicbell-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.magicbell.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  2 01:23:11 2026 GMT\n  hsts: null\n- host: api.magicbell.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  2 01:23:11 2026 GMT\n  hsts: null\ndomains:\n- domain: magicbell.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/magicbell/refs/heads/main/security/magicbell-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- notifications
- push notifications
- in-app notifications
- email
- SMS
- Slack
- Microsoft Teams
- webhooks
- notification inbox
- multichannel
- mobile push
- web push
---
