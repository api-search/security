---
api_specs:
- filename: yutori-openapi-original.json
  format: json
  label: Yutori API
  slug: yutori-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/yutori/refs/heads/main/openapi/yutori-openapi-original.json
description: ''
domains:
- caa:
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  - 0 issue "amazon.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: yutori.com
  spf: true
hosts:
- cert_expires: Aug 26 12:53:30 2026 GMT
  host: yutori.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 18 23:59:59 2026 GMT
  host: api.yutori.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Yutori Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Yutori, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Yutori
provider_slug: yutori
slug: yutori-domain-security
source_filename: yutori-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: yutori.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 26 12:53:30 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.yutori.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 18 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: yutori.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/yutori/refs/heads/main/security/yutori-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- AI
- Agents
- Web Automation
- Browser Automation
- Web Monitoring
- Research
- MCP
- LLM
---
