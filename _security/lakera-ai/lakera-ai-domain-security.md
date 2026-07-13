---
api_specs:
- filename: lakera-guard-api-openapi.yml
  format: yaml
  label: Lakera Guard API
  slug: lakera-guard-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lakera-ai/refs/heads/main/openapi/lakera-guard-api-openapi.yml
- filename: lakera-platform-api-openapi.yml
  format: yaml
  label: Lakera Platform API
  slug: lakera-platform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lakera-ai/refs/heads/main/openapi/lakera-platform-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "amazon.com"
  - 0 issue "amazonaws.com"
  - 0 issue "amazontrust.com"
  - 0 issue "awstrust.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: lakera.ai
  spf: true
hosts:
- cert_expires: Sep 11 01:18:44 2026 GMT
  host: www.lakera.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec  2 23:59:59 2026 GMT
  host: platform.lakera.ai
  hsts: true
  hsts_max_age: 31556926
  https: true
  tls_version: TLSv1.2
- cert_expires: Sep 12 10:00:39 2026 GMT
  host: docs.lakera.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Lakera Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Lakera, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Lakera
provider_slug: lakera-ai
slug: lakera-ai-domain-security
source_filename: lakera-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.lakera.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 11 01:18:44 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: platform.lakera.ai\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec  2 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31556926\n- host: docs.lakera.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 12 10:00:39 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: lakera.ai\n  dnssec: false\n  caa:\n  - 0 issue \"amazon.com\"\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"amazontrust.com\"\n  - 0 issue \"awstrust.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lakera-ai/refs/heads/main/security/lakera-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- AI Security
- Artificial Intelligence
- Generative AI
- LLM Security
- Prompt Injection
- AI Guardrails
- AI Red Teaming
- Data Loss Prevention
- Content Moderation
- Check Point
---
