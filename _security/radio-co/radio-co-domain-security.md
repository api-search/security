---
api_specs:
- filename: radio-co-openapi.yml
  format: yaml
  label: Radio.co
  slug: radio-co
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/radio-co/refs/heads/main/openapi/radio-co-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: radio.co
  spf: true
hosts:
- cert_expires: Oct  2 18:45:06 2026 GMT
  host: radio.co
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 18 14:31:37 2026 GMT
  host: public.radio.co
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Radio Co Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Radio.co, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Radio.co
provider_slug: radio-co
slug: radio-co-domain-security
source_filename: radio-co-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: radio.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 18:45:06 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: public.radio.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 18 14:31:37 2026 GMT\n  hsts: null\ndomains:\n- domain: radio.co\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/radio-co/refs/heads/main/security/radio-co-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Radio
- Streaming
- Audio
- Music
---
