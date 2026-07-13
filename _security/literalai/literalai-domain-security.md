---
api_specs:
- filename: literalai-openapi.yml
  format: yaml
  label: Literal AI Threads & Steps API
  slug: threads-steps
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/literalai/refs/heads/main/openapi/literalai-openapi.yml
- filename: literalai-openapi.yml
  format: yaml
  label: Literal AI Generations API
  slug: generations
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/literalai/refs/heads/main/openapi/literalai-openapi.yml
- filename: literalai-openapi.yml
  format: yaml
  label: Literal AI Datasets API
  slug: datasets
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/literalai/refs/heads/main/openapi/literalai-openapi.yml
- filename: literalai-openapi.yml
  format: yaml
  label: Literal AI Experiments API
  slug: experiments
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/literalai/refs/heads/main/openapi/literalai-openapi.yml
- filename: literalai-openapi.yml
  format: yaml
  label: Literal AI Prompts API
  slug: prompts
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/literalai/refs/heads/main/openapi/literalai-openapi.yml
- filename: literalai-openapi.yml
  format: yaml
  label: Literal AI Scores API
  slug: scores
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/literalai/refs/heads/main/openapi/literalai-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: literalai.com
  spf: false
- caa: []
  dmarc: false
  dnssec: false
  domain: getliteral.ai
  spf: false
hosts:
- host: www.literalai.com
  https: false
- cert_expires: Sep 30 07:37:55 2026 GMT
  host: docs.literalai.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  7 03:39:38 2026 GMT
  host: cloud.getliteral.ai
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Literalai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Literal AI, probed live across 3 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=quarantine).'
provider_name: Literal AI
provider_slug: literalai
slug: literalai-domain-security
source_filename: literalai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.literalai.com\n  https: false\n- host: docs.literalai.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 07:37:55 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: cloud.getliteral.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  7 03:39:38 2026 GMT\n  hsts: null\ndomains:\n- domain: literalai.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: getliteral.ai\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/literalai/refs/heads/main/security/literalai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- AI
- LLM
- Observability
- Evaluation
- Monitoring
---
