---
description: ''
domains:
- caa:
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "ssl.com"
  - 0 issuewild "comodoca.com"
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: startupbuffer.com
  spf: true
hosts:
- cert_expires: Sep  4 17:57:53 2026 GMT
  host: startupbuffer.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Startup Buffer Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Startup Buffer, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Startup Buffer
provider_slug: startup-buffer
slug: startup-buffer-domain-security
source_filename: startup-buffer-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: startupbuffer.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  4 17:57:53 2026 GMT\n  hsts: null\ndomains:\n- domain: startupbuffer.com\n  dnssec: true\n  caa:\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"comodoca.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/startup-buffer/refs/heads/main/security/startup-buffer-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Directory
- Product Discovery
- Startups
- Listing
- Community
---
