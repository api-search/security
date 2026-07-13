---
api_specs:
- filename: snorkel-ai-openapi.yml
  format: yaml
  label: Snorkel Flow SDK / Platform
  slug: snorkel-flow-sdk-platform
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/snorkel-ai/refs/heads/main/openapi/snorkel-ai-openapi.yml
- filename: snorkel-ai-openapi.yml
  format: yaml
  label: Programmatic Labeling
  slug: programmatic-labeling
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/snorkel-ai/refs/heads/main/openapi/snorkel-ai-openapi.yml
- filename: snorkel-ai-openapi.yml
  format: yaml
  label: Evaluation
  slug: evaluation
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/snorkel-ai/refs/heads/main/openapi/snorkel-ai-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: snorkel.ai
  spf: true
hosts:
- cert_expires: Aug 10 21:55:11 2026 GMT
  host: snorkel.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  3 07:23:46 2026 GMT
  host: docs.snorkel.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Snorkel Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Snorkel AI, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Snorkel AI
provider_slug: snorkel-ai
slug: snorkel-ai-domain-security
source_filename: snorkel-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: snorkel.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 10 21:55:11 2026 GMT\n  hsts: false\n- host: docs.snorkel.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  3 07:23:46 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: snorkel.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/snorkel-ai/refs/heads/main/security/snorkel-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- AI
- Data Development
- Programmatic Labeling
- Weak Supervision
- Evaluation
- SDK
---
