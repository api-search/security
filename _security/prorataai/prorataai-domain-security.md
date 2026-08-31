---
api_specs:
- filename: prorataai-chat-api-openapi.yml
  format: yaml
  label: ProRata.ai Chat API
  slug: prorataai-chat-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/prorataai/refs/heads/main/openapi/prorataai-chat-api-openapi.yml
- filename: prorataai-health-api-openapi.yml
  format: yaml
  label: ProRata.ai Health API
  slug: prorataai-health-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/prorataai/refs/heads/main/openapi/prorataai-health-api-openapi.yml
- filename: prorataai-publishers-api-openapi.yml
  format: yaml
  label: ProRata.ai Publishers API
  slug: prorataai-publishers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/prorataai/refs/heads/main/openapi/prorataai-publishers-api-openapi.yml
- filename: prorataai-questions-api-openapi.yml
  format: yaml
  label: ProRata.ai Questions API
  slug: prorataai-questions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/prorataai/refs/heads/main/openapi/prorataai-questions-api-openapi.yml
- filename: prorataai-root-api-openapi.yml
  format: yaml
  label: ProRata.ai Root API
  slug: prorataai-root-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/prorataai/refs/heads/main/openapi/prorataai-root-api-openapi.yml
- filename: prorataai-summaries-api-openapi.yml
  format: yaml
  label: ProRata.ai Summaries API
  slug: prorataai-summaries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/prorataai/refs/heads/main/openapi/prorataai-summaries-api-openapi.yml
- filename: prorataai-threads-api-openapi.yml
  format: yaml
  label: ProRata.ai Threads API
  slug: prorataai-threads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/prorataai/refs/heads/main/openapi/prorataai-threads-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: prorata.ai
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: gist.ai
  spf: true
hosts:
- cert_expires: Nov 22 20:45:06 2026 GMT
  host: prorata.ai
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 19 12:31:12 2026 GMT
  host: platform.gist.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 10 10:40:20 2026 GMT
  host: api.gist.ai
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Prorataai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ProRata.ai, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: ProRata.ai
provider_slug: prorataai
slug: prorataai-domain-security
source_filename: prorataai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: prorata.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 22 20:45:06 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\n- host: platform.gist.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 19 12:31:12 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.gist.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 10 10:40:20 2026 GMT\n  hsts: null\ndomains:\n- domain: prorata.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: gist.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/prorataai/refs/heads/main/security/prorataai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Artificial Intelligence
- Search
- Content
- Publishing
- Advertising
- Attribution
- Answer Engines
- Generative AI
- Media
- Content Licensing
---
