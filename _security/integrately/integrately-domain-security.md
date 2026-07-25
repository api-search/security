---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: integrately.com
  spf: true
hosts:
- cert_expires: Oct  3 14:15:07 2026 GMT
  host: integrately.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 14 03:33:46 2026 GMT
  host: app.integrately.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Integrately Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Integrately, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Integrately
provider_slug: integrately
slug: integrately-domain-security
source_filename: integrately-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: integrately.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 14:15:07 2026 GMT\n  hsts: false\n- host: app.integrately.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 03:33:46 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: integrately.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/integrately/refs/heads/main/security/integrately-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Automation
- Business Process Automation
- iPaaS
- No-Code
- SaaS Integration
- SMB
- Triggers and Actions
- Webhooks
- Workflow Automation
- Workflows
---
