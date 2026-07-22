---
description: ''
domains:
- caa:
  - 0 issue "pki.goog"
  - 0 issue "sectigo.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: moda.dev
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: workers.dev
  spf: true
hosts:
- cert_expires: Sep 14 09:32:14 2026 GMT
  host: moda.dev
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 14 09:32:14 2026 GMT
  host: docs.moda.dev
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 29 07:27:25 2026 GMT
  host: moda-ingest.modas.workers.dev
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Moda Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Moda, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Moda
provider_slug: moda
slug: moda-domain-security
source_filename: moda-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: moda.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 09:32:14 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.moda.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 09:32:14 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: moda-ingest.modas.workers.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 07:27:25 2026 GMT\n  hsts: null\ndomains:\n- domain: moda.dev\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: workers.dev\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/moda/refs/heads/main/security/moda-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- AI Agents
- LLM Observability
- Agent Analytics
- Continual Learning
- Monitoring
- Developer Tools
- MCP
- OpenTelemetry
- Prompt Management
- Y Combinator
---
