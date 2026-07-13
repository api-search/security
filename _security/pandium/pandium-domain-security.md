---
api_specs:
- filename: pandium-pandium-openapi.yml
  format: yaml
  label: Pandium
  slug: pandium
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pandium/refs/heads/main/openapi/pandium-pandium-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: pandium.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: pandium.io
  spf: false
hosts:
- cert_expires: Sep 29 08:09:37 2026 GMT
  host: www.pandium.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 11 09:42:35 2026 GMT
  host: api.pandium.io
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  2 15:36:48 2026 GMT
  host: api.sandbox.pandium.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Pandium Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Pandium, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Pandium
provider_slug: pandium
slug: pandium-domain-security
source_filename: pandium-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.pandium.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 08:09:37 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.pandium.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 11 09:42:35 2026 GMT\n  hsts: null\n- host: api.sandbox.pandium.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  2 15:36:48 2026 GMT\n  hsts: null\ndomains:\n- domain: pandium.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: pandium.io\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pandium/refs/heads/main/security/pandium-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- B2B
- Hubs
- Integrations
- Workflows
---
