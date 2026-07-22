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
  dmarc_policy: quarantine
  dnssec: false
  domain: motley.ai
  spf: true
hosts:
- cert_expires: Aug  8 13:55:00 2026 GMT
  host: motley.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 19 12:24:51 2026 GMT
  host: docs.motley.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 19 12:24:51 2026 GMT
  host: app.motley.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Motley Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Motley, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Motley
provider_slug: motley
slug: motley-domain-security
source_filename: motley-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: motley.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug  8 13:55:00 2026 GMT\n  hsts: false\n- host: docs.motley.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 19 12:24:51 2026 GMT\n  hsts: false\n- host: app.motley.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 19 12:24:51 2026 GMT\n  hsts: false\ndomains:\n- domain: motley.ai\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/motley/refs/heads/main/security/motley-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Semantic Layer
- Business Intelligence
- Analytics
- AI Agents
- MCP
- SQL
- Data
- Reporting
---
