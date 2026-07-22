---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: convey.dev
  spf: true
hosts:
- cert_expires: Oct 14 02:25:12 2026 GMT
  host: convey.dev
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Convey Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Convey, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Convey
provider_slug: convey
slug: convey-domain-security
source_filename: convey-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: convey.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 14 02:25:12 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: convey.dev\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/convey/refs/heads/main/security/convey-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Artificial Intelligence
- AI Agents
- Automation
- Enterprise
- Workflow Automation
- Digital Workers
- Operations
---
