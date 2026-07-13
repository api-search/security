---
description: ''
domains:
- caa:
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "ssl.com"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: middleware.io
  spf: true
hosts:
- cert_expires: Sep 23 02:07:23 2026 GMT
  host: middleware.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  1 09:37:13 2026 GMT
  host: app.middleware.io
  hsts: true
  hsts_max_age: 2592000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Middleware Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Middleware, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Middleware
provider_slug: middleware
slug: middleware-domain-security
source_filename: middleware-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: middleware.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 23 02:07:23 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: app.middleware.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 09:37:13 2026 GMT\n  hsts: true\n  hsts_max_age: 2592000\ndomains:\n- domain: middleware.io\n  dnssec: true\n  caa:\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/middleware/refs/heads/main/security/middleware-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- AI Operations
- APM
- API Monitoring
- Container Monitoring
- Database Monitoring
- Infrastructure Monitoring
- LLM Observability
- Log Management
- Observability
- Real User Monitoring
- Synthetic Monitoring
---
