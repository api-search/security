---
api_specs:
- filename: stepfun-realtime-asyncapi.yml
  format: yaml
  label: StepFun Realtime API
  slug: realtime-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/stepfun/refs/heads/main/asyncapi/stepfun-realtime-asyncapi.yml
description: ''
domains:
- caa:
  - redirect.stepfun.com.
  dmarc: false
  dnssec: true
  domain: stepfun.com
  spf: true
hosts:
- cert_expires: Nov 14 23:59:59 2026 GMT
  host: www.stepfun.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 14 23:59:59 2026 GMT
  host: platform.stepfun.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 14 23:59:59 2026 GMT
  host: api.stepfun.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Stepfun Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for StepFun, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC absent.'
provider_name: StepFun
provider_slug: stepfun
slug: stepfun-domain-security
source_filename: stepfun-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.stepfun.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 14 23:59:59 2026 GMT\n  hsts: false\n- host: platform.stepfun.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 14 23:59:59 2026 GMT\n  hsts: false\n- host: api.stepfun.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 14 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: stepfun.com\n  dnssec: true\n  caa:\n  - redirect.stepfun.com.\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/stepfun/refs/heads/main/security/stepfun-domain-security.yml
summary_line: TLSv1.3 · DNSSEC
tags:
- AI
- Artificial Intelligence
- LLM
- Multimodal
- Chat Completion
- Audio
- Speech
- Text to Speech
- Speech Recognition
- Images
- Realtime
- Vector Stores
- China
---
