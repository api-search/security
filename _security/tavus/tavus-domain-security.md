---
api_specs:
- filename: tavus-openapi.yml
  format: yaml
  label: Tavus API
  slug: tavus-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tavus/refs/heads/main/openapi/tavus-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: tavus.io
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: tavusapi.com
  spf: false
hosts:
- cert_expires: Aug 17 18:42:34 2026 GMT
  host: www.tavus.io
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  2 13:47:37 2026 GMT
  host: docs.tavus.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 23 23:59:59 2026 GMT
  host: tavusapi.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Tavus Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Tavus, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Tavus
provider_slug: tavus
slug: tavus-domain-security
source_filename: tavus-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.tavus.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 17 18:42:34 2026 GMT\n  hsts: false\n- host: docs.tavus.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  2 13:47:37 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: tavusapi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 23 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: tavus.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: tavusapi.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tavus/refs/heads/main/security/tavus-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Artificial Intelligence
- Generative AI
- Video
- Conversational AI
- Avatars
- Replicas
- Personalization
- Real Time
- CVI
- Webhooks
---
