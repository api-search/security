---
description: ''
domains:
- caa:
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "globalsign.com"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "sectigo.com"
  - 0 issuewild "ssl.com"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: botinfo.ai
  spf: true
hosts:
- cert_expires: Dec 13 21:04:02 2026 GMT
  host: botinfo.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Botinfo Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for BotInfo AI, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: BotInfo AI
provider_slug: botinfo-ai
slug: botinfo-ai-domain-security
source_filename: botinfo-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: botinfo.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 13 21:04:02 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: botinfo.ai\n  dnssec: false\n  caa:\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"globalsign.com\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"sectigo.com\"\n  - 0 issuewild \"ssl.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/botinfo-ai/security/botinfo-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Lead Intelligence
- Market Intelligence
- Referral Service
---
