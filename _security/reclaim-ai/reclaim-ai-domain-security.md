---
api_specs:
- filename: reclaim-api-0.1.yml
  format: yaml
  label: Reclaim API
  slug: reclaim-api
  spec_type: OpenAPI
  url: https://api.app.reclaim.ai/swagger/reclaim-api-0.1.yml
description: ''
domains:
- caa:
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  - 0 issue "amazon.com"
  - 0 issue "comodoca.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: reclaim.ai
  spf: true
hosts:
- cert_expires: Sep  6 08:46:12 2026 GMT
  host: reclaim.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 25 20:55:18 2026 GMT
  host: help.reclaim.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Mar  5 23:59:59 2027 GMT
  host: api.app.reclaim.ai
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Reclaim Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Reclaim.ai, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Reclaim.ai
provider_slug: reclaim-ai
slug: reclaim-ai-domain-security
source_filename: reclaim-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: reclaim.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  6 08:46:12 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: help.reclaim.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 25 20:55:18 2026 GMT\n  hsts: false\n- host: api.app.reclaim.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar  5 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: reclaim.ai\n  dnssec: false\n  caa:\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"comodoca.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/reclaim-ai/refs/heads/main/security/reclaim-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- AI
- Scheduling
- Calendar
- Productivity
- Tasks
- Habits
- Time Management
- Meetings
- Focus Time
---
