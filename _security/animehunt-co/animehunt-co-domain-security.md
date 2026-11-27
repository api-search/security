---
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "sectigo.com"
  - 0 issue "ssl.com"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: animehunt.co
  spf: true
hosts:
- cert_expires: Jan 10 05:23:43 2027 GMT
  host: animehunt.co
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: AnimeHunt Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AnimeHunt, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: AnimeHunt
provider_slug: animehunt-co
slug: animehunt-co-domain-security
source_filename: animehunt-co-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-01'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: animehunt.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 10 05:23:43 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: animehunt.co\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/animehunt-co/security/animehunt-co-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Anime
- Manga
- Webtoons
- Discovery
- Tracker
---
