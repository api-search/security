---
description: ''
domains:
- caa:
  - 0 issue "amazon.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "globalsign.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: once.com
  spf: true
hosts:
- cert_expires: Jan  1 14:44:44 2027 GMT
  host: once.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Campfire 37Signals Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Campfire, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Campfire
provider_slug: campfire-37signals
slug: campfire-37signals-domain-security
source_filename: campfire-37signals-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-27'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: once.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  1 14:44:44 2027 GMT\n  hsts: false\ndomains:\n- domain: once.com\n  dnssec: false\n  caa:\n  - 0 issue \"amazon.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"globalsign.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/campfire-37signals/security/campfire-37signals-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Chat
- OpenSource
- SelfHosted
- Collaboration
- Privacy
---
