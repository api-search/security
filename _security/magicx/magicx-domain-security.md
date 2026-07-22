---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: magicx.ai
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: ai-autocomplete.com
  spf: true
hosts:
- cert_expires: Aug 28 22:26:40 2026 GMT
  host: magicx.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  7 23:59:59 2026 GMT
  host: ai-autocomplete.com
  hsts: true
  hsts_max_age: 10886400
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 21 07:30:29 2026 GMT
  host: api.ai-autocomplete.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Magicx Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for MagicX, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: MagicX
provider_slug: magicx
slug: magicx-domain-security
source_filename: magicx-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: magicx.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 28 22:26:40 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: ai-autocomplete.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  7 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 10886400\n- host: api.ai-autocomplete.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 21 07:30:29 2026 GMT\n  hsts: null\ndomains:\n- domain: magicx.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: ai-autocomplete.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/magicx/refs/heads/main/security/magicx-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- AI
- Autocomplete
- Developer Tools
- SDK
- Natural Language
- Productivity
- Machine Learning
---
