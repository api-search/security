---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: locale.ai
  spf: true
hosts:
- cert_expires: Sep 23 08:15:40 2026 GMT
  host: locale.ai
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Locale Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Locale, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Locale
provider_slug: locale
slug: locale-domain-security
source_filename: locale-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: locale.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 23 08:15:40 2026 GMT\n  hsts: null\ndomains:\n- domain: locale.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/locale/refs/heads/main/security/locale-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Workflow Automation
- No-Code
- Integration
- iPaaS
- Operations
- Productivity
- AI Actions
---
