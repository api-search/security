---
description: ''
domains:
- caa:
  - 0 issuewild "ssl.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "ssl.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: mcsrvstat.us
  spf: true
hosts:
- cert_expires: Aug 12 05:38:20 2026 GMT
  host: api.mcsrvstat.us
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Minecraft Server Status Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Minecraft Server Status, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Minecraft Server Status
provider_slug: minecraft-server-status
slug: minecraft-server-status-domain-security
source_filename: minecraft-server-status-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: api.mcsrvstat.us\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 12 05:38:20 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: mcsrvstat.us\n  dnssec: true\n  caa:\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/minecraft-server-status/refs/heads/main/security/minecraft-server-status-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Games And Comics
- Public APIs
---
