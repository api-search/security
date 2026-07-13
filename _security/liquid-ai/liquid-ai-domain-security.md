---
description: ''
domains:
- caa:
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  - 0 iodef "security@liquid.ai"
  - 0 issue "amazon.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: liquid.ai
  spf: true
hosts:
- cert_expires: Sep 25 15:16:07 2026 GMT
  host: www.liquid.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 25 03:36:46 2026 GMT
  host: docs.liquid.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 22 22:01:29 2026 GMT
  host: api.liquid.ai
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Liquid Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Liquid AI, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Liquid AI
provider_slug: liquid-ai
slug: liquid-ai-domain-security
source_filename: liquid-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.liquid.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 25 15:16:07 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.liquid.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 25 03:36:46 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.liquid.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 22 22:01:29 2026 GMT\n  hsts: null\ndomains:\n- domain: liquid.ai\n  dnssec: true\n  caa:\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  - 0 iodef \"security@liquid.ai\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/liquid-ai/refs/heads/main/security/liquid-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- AI
- LLM
- Inference
- Foundation Models
- Liquid Networks
- Edge AI
- On-Device
---
