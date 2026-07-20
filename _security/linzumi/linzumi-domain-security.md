---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: linzumi.com
  spf: false
- caa:
  - 0 issuewild "sectigo.com"
  - 0 issuewild "ssl.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: npmjs.com
  spf: true
hosts:
- cert_expires: Sep 22 18:47:17 2026 GMT
  host: linzumi.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 12 04:22:28 2026 GMT
  host: www.npmjs.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 23 04:04:40 2026 GMT
  host: serve.linzumi.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Linzumi Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Linzumi, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: Linzumi
provider_slug: linzumi
slug: linzumi-domain-security
source_filename: linzumi-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: linzumi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 22 18:47:17 2026 GMT\n  hsts: false\n- host: www.npmjs.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 12 04:22:28 2026 GMT\n  hsts: null\n- host: serve.linzumi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 23 04:04:40 2026 GMT\n  hsts: false\ndomains:\n- domain: linzumi.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n- domain: npmjs.com\n  dnssec: true\n  caa:\n  - 0 issuewild \"sectigo.com\"\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/linzumi/refs/heads/main/security/linzumi-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
- Artificial Intelligence
- Developer Tools
- Coding Agents
- Team Chat
- Collaboration
- MCP
- Command Line Interface
- Y Combinator
---
