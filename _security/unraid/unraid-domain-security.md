---
description: ''
domains:
- caa:
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "ssl.com"
  - 0 issuewild "amazon.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: unraid.net
  spf: true
hosts:
- cert_expires: Dec 29 15:46:45 2026 GMT
  host: unraid.net
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Unraid Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Unraid, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Unraid
provider_slug: unraid
slug: unraid-domain-security
source_filename: unraid-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: unraid.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 29 15:46:45 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: unraid.net\n  dnssec: false\n  caa:\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"amazon.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/unraid/security/unraid-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Operating System
- Network‑Attached Storage
- Docker
- Virtual Machines
- Self‑Hosting
- Homelab
---
