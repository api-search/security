---
description: ''
domains:
- caa:
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "ssl.com"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: you.com
  spf: true
hosts:
- cert_expires: Aug 15 19:41:50 2026 GMT
  host: you.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 22 21:10:42 2026 GMT
  host: api.you.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: You Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for You.com, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: You.com
provider_slug: you-com
slug: you-com-domain-security
source_filename: you-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: you.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 15 19:41:50 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.you.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 22 21:10:42 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: you.com\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/you-com/refs/heads/main/security/you-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Search
- AI Search
- LLMs
- AI Agents
- Research
- News
- Finance
- Web Index
- Real-Time
- SOC 2
---
