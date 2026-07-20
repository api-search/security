---
api_specs:
- filename: arpeggi-labs-kits-openapi.yml
  format: yaml
  label: Kits AI API
  slug: kits-ai-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/arpeggi-labs/refs/heads/main/openapi/arpeggi-labs-kits-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: kits.ai
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: arpeggi.io
  spf: true
hosts:
- cert_expires: Sep 27 15:02:06 2026 GMT
  host: kits.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 28 14:56:20 2026 GMT
  host: docs.kits.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Mar 18 23:59:59 2027 GMT
  host: arpeggi.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Arpeggi Labs Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Arpeggi Labs, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Arpeggi Labs
provider_slug: arpeggi-labs
slug: arpeggi-labs-domain-security
source_filename: arpeggi-labs-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: kits.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 27 15:02:06 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.kits.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 28 14:56:20 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: arpeggi.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 18 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: kits.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: arpeggi.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/arpeggi-labs/refs/heads/main/security/arpeggi-labs-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Music
- Audio
- Artificial Intelligence
- Voice
- Machine Learning
- Generative AI
- Media
---
