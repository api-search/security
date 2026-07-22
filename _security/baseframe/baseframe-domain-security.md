---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: baseframe.co
  spf: true
hosts:
- cert_expires: Oct  1 10:58:04 2026 GMT
  host: baseframe.co
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Baseframe Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Baseframe, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Baseframe
provider_slug: baseframe
slug: baseframe-domain-security
source_filename: baseframe-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: baseframe.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 10:58:04 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: baseframe.co\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/baseframe/refs/heads/main/security/baseframe-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Artificial Intelligence
- Automation
- Workflow Discovery
- Productivity
- Process Mining
- Desktop Application
- Y Combinator
---
