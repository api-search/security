---
description: ''
domains:
- caa:
  - 0 issuewild "sectigo.com"
  - 0 issuewild "ssl.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "globalsign.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: amanahagent.cloud
  spf: true
hosts:
- cert_expires: Aug 23 23:59:59 2026 GMT
  host: sunnah.amanahagent.cloud
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Amanah Sunnah Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Amanah Sunnah, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Amanah Sunnah
provider_slug: amanah-sunnah
slug: amanah-sunnah-domain-security
source_filename: amanah-sunnah-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: sunnah.amanahagent.cloud\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 23 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: amanahagent.cloud\n  dnssec: false\n  caa:\n  - 0 issuewild \"sectigo.com\"\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"globalsign.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amanah-sunnah/refs/heads/main/security/amanah-sunnah-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Books
- Public APIs
---
