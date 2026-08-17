---
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 issue "sectigo.com"
  - 0 issue "amazon.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: expertise.ai
  spf: true
hosts:
- cert_expires: Sep 14 19:15:05 2026 GMT
  host: www.expertise.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 14 19:15:05 2026 GMT
  host: my.expertise.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 14 19:15:05 2026 GMT
  host: docs.expertise.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  5 20:57:49 2026 GMT
  cert_verify: 0 (ok)
  host: api.expertise.ai
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 31536000
  https: true
  note: 'Added by hand on 2026-08-13 — probe-domain-security.py did not pick up the API host. This is the host that serves both the documented REST base URL (/v0/users) and the remote MCP endpoint (/mcp). It also returns a full security header set on every response including 404s: content-security-policy default-src ''self'', x-frame-options SAMEORIGIN, x-content-type-options nosniff, referrer-policy strict-origin-when-cross-origin.'
  tls_version: TLSv1.3
- cert_expires: Oct 15 17:27:54 2026 GMT
  host: cdn.expertise.ai
  hsts: false
  https: true
  note: Added by hand on 2026-08-13. Serves the Expertise Live web-component runtime bundle and styles. No HSTS header.
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Chatsimple Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Chatsimple, probed live across 5 host(s) and 1 registrable domain(s). 5 host(s) serve HTTPS (up to TLSv1.3); 4 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Chatsimple
provider_slug: chatsimple
slug: chatsimple-domain-security
source_filename: chatsimple-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.expertise.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 19:15:05 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: my.expertise.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 19:15:05 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.expertise.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 19:15:05 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.expertise.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  5 20:57:49 2026 GMT\n  cert_verify: 0 (ok)\n  hsts: true\n  hsts_max_age: 31536000\n  hsts_include_subdomains: true\n  note: >-\n    Added by hand on 2026-08-13 — probe-domain-security.py did not pick up the\n    API host. This is the host that serves both the documented REST base URL\n    (/v0/users) and the remote MCP endpoint (/mcp). It also returns\
  \ a full\n    security header set on every response including 404s:\n    content-security-policy default-src 'self', x-frame-options SAMEORIGIN,\n    x-content-type-options nosniff, referrer-policy strict-origin-when-cross-origin.\n- host: cdn.expertise.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 15 17:27:54 2026 GMT\n  hsts: false\n  note: >-\n    Added by hand on 2026-08-13. Serves the Expertise Live web-component runtime\n    bundle and styles. No HSTS header.\ndomains:\n- domain: expertise.ai\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"amazon.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/chatsimple/refs/heads/main/security/chatsimple-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- AI Agents
- Conversational AI
- Chatbot
- Lead Generation
- Sales Automation
- CRM Integration
- Voice AI
- Go-To-Market
- Customer Engagement
---
