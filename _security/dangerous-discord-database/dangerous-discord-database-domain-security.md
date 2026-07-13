---
description: ''
domains:
- caa:
  - 0 issue "ssl.com"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  dmarc: false
  dnssec: true
  domain: riverside.rocks
  spf: true
hosts:
- host: discord.riverside.rocks
  https: false
kind: domain-security
layout: security
method: probed
name: Dangerous Discord Database Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Dangerous Discord Database, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC present, SPF present, DMARC absent.'
provider_name: Dangerous Discord Database
provider_slug: dangerous-discord-database
slug: dangerous-discord-database-domain-security
source_filename: dangerous-discord-database-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: discord.riverside.rocks\n  https: false\ndomains:\n- domain: riverside.rocks\n  dnssec: true\n  caa:\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dangerous-discord-database/refs/heads/main/security/dangerous-discord-database-domain-security.yml
summary_line: DNSSEC
tags:
- Social
- Public APIs
---
