---
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "ssl.com"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: demostack.com
  spf: true
hosts:
- cert_expires: Oct 17 11:16:18 2026 GMT
  host: www.demostack.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  9 01:22:41 2026 GMT
  host: api.demostack.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Demostack Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Demostack, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Demostack
provider_slug: demostack
slug: demostack-domain-security
source_filename: demostack-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-14'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.demostack.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 17 11:16:18 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.demostack.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  9 01:22:41 2026 GMT\n  hsts: false\ndomains:\n- domain: demostack.com\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/demostack/refs/heads/main/security/demostack-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Sales Demo
- Demo Automation
- Product Simulation
- Webhooks
- CRM Integration
- Sales Enablement
- Presales
- Sales Engineering
- Analytics
- AI
- MCP
---
