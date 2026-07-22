---
description: ''
domains:
- caa:
  - 0 issue "pki.goog"
  - 0 issue "sectigo.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: cofounder.co
  spf: false
hosts:
- cert_expires: Sep 30 20:21:16 2026 GMT
  host: cofounder.co
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: General Intelligence Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for General Intelligence, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=reject).'
provider_name: General Intelligence
provider_slug: general-intelligence
slug: general-intelligence-domain-security
source_filename: general-intelligence-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: cofounder.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 20:21:16 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: cofounder.co\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: false\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/general-intelligence/refs/heads/main/security/general-intelligence-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Artificial Intelligence
- AI Agents
- Agent Orchestration
- Business Automation
- No-Code
- Startup
- New York
---
