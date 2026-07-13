---
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issuewild "ssl.com"
  - 0 issue "certainly.com"
  - 0 issue "pki.goog;cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  - 0 issue "ssl.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: lindy.ai
  spf: true
hosts:
- cert_expires: Sep 14 19:30:14 2026 GMT
  host: www.lindy.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Lindy Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Lindy, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Lindy
provider_slug: lindy
slug: lindy-domain-security
source_filename: lindy-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.lindy.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 19:30:14 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: lindy.ai\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"certainly.com\"\n  - 0 issue \"pki.goog;cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issue \"ssl.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lindy/refs/heads/main/security/lindy-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- AI Agents
- AI Automation
---
