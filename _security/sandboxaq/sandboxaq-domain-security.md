---
api_specs:
- filename: sandboxaq-flint-ai-platform-openapi.json
  format: json
  label: Flint AI Platform API
  slug: flint-ai-platform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sandboxaq/refs/heads/main/openapi/sandboxaq-flint-ai-platform-openapi.json
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "sectigo.com"
  - 0 issuewild "amazonaws.com"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: sandboxaq.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: flintai.dev
  spf: true
hosts:
- cert_expires: Oct  2 21:09:49 2026 GMT
  host: www.sandboxaq.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 13 14:23:53 2026 GMT
  host: docs.flintai.dev
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- host: your-instance.flintai.dev
  https: false
kind: domain-security
layout: security
method: probed
name: Sandboxaq Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for SandboxAQ, probed live across 3 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: SandboxAQ
provider_slug: sandboxaq
slug: sandboxaq-domain-security
source_filename: sandboxaq-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.sandboxaq.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 21:09:49 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.flintai.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 13 14:23:53 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: your-instance.flintai.dev\n  https: false\ndomains:\n- domain: sandboxaq.com\n  dnssec: true\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"sectigo.com\"\n  - 0 issuewild \"amazonaws.com\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: flintai.dev\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sandboxaq/refs/heads/main/security/sandboxaq-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Artificial Intelligence
- Security
- Cryptography
- Post-Quantum Cryptography
- Agents
- Model Context Protocol
- Simulation
- Drug Discovery
- Materials Science
- AI Security
- Quantum
---
