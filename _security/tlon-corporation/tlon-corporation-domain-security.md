---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: tlon.io
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: urbit.org
  spf: true
hosts:
- cert_expires: Oct  3 19:01:38 2026 GMT
  host: tlon.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 27 22:14:06 2026 GMT
  host: docs.urbit.org
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 23 23:06:38 2026 GMT
  host: tlon.network
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Tlon Corporation Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Tlon Corporation, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Tlon Corporation
provider_slug: tlon-corporation
slug: tlon-corporation-domain-security
source_filename: tlon-corporation-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: tlon.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 19:01:38 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.urbit.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 27 22:14:06 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: tlon.network\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 23 23:06:38 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: tlon.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: urbit.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tlon-corporation/refs/heads/main/security/tlon-corporation-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Messaging
- Social
- Urbit
- Self-Hosting
- Decentralization
- Agents
- MCP
- Chat
- Hosting
---
