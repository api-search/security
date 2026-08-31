---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: weaveapi.dev
  spf: true
hosts:
- cert_expires: Nov  5 15:14:29 2026 GMT
  host: weaveapi.dev
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 29 11:42:07 2026 GMT
  host: api.weaveapi.dev
  hsts: true
  hsts_correction_note: 'The automated probe recorded hsts: null for this host because api.weaveapi.dev answers HEAD / with a bare 404. Direct header inspection on 2026-08-11 confirms the header IS served on every response including the 404 and the 401: "strict-transport-security: max-age=31536000; includeSubDomains". Corrected from observed evidence.'
  hsts_include_subdomains: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Weaveapi Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for WeaveAPI - OpenAI-compatible AI API Gateway, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: WeaveAPI - OpenAI-compatible AI API Gateway
provider_slug: weaveapi
slug: weaveapi-domain-security
source_filename: weaveapi-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: weaveapi.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  5 15:14:29 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.weaveapi.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 29 11:42:07 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n  hsts_include_subdomains: true\n  hsts_correction_note: >-\n    The automated probe recorded hsts: null for this host because api.weaveapi.dev answers HEAD / with\n    a bare 404. Direct header inspection on 2026-08-11 confirms the header IS served on every response\n    including the 404 and the 401: \"strict-transport-security: max-age=31536000; includeSubDomains\".\n    Corrected from observed evidence.\ndomains:\n- domain: weaveapi.dev\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n\nfindings:\n  strengths:\n    - TLS 1.3 on both the marketing\
  \ host and the API host.\n    - HSTS with a one-year max-age and includeSubDomains on both hosts.\n    - SPF and DMARC published, with DMARC at p=quarantine.\n    - >-\n      Additional response hardening on the API host — x-content-type-options nosniff and\n      referrer-policy strict-origin-when-cross-origin.\n  gaps:\n    - No DNSSEC on weaveapi.dev.\n    - No CAA records — any public CA may issue for the domain.\n    - DMARC is p=quarantine rather than p=reject.\n    - Certificates are short-dated (Oct/Nov 2026) — normal for automated issuance, noted for currency.\n  note: >-\n    Transport posture is solid and is the strongest area of WeaveAPI's security surface. It stands in\n    contrast to the application layer, where there is no security.txt, no vulnerability disclosure\n    channel, no trust center and no published compliance program (see conformance/ and well-known/).\n\nx-evidence:\n  - url: https://api.weaveapi.dev/v1/models\n    http_status: 401\n    header_observed: 'strict-transport-security:\
  \ max-age=31536000; includeSubDomains'\n  - url: https://weaveapi.dev/\n    http_status: 200\n    header_observed: 'strict-transport-security: max-age=31536000; includeSubDomains'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/weaveapi/refs/heads/main/security/weaveapi-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Artificial Intelligence
- LLM
- AI inference
- API gateway
- aggregator
- OpenAI-compatible
- Developer Tools
- model routing
- LLM gateway
- prepaid credits
- agent tools
- model marketplace
---
