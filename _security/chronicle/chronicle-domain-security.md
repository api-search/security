---
description: ''
domains:
- caa:
  - 0 issue "amazonaws.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "ssl.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: chroniclehq.com
  spf: true
hosts:
- cert_expires: Oct  9 06:59:25 2026 GMT
  host: chroniclehq.com
  hsts: true
  hsts_max_age: 2592000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 30 06:17:53 2026 GMT
  host: docs.chroniclehq.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec  7 23:59:59 2026 GMT
  host: api.chroniclehq.com
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Chronicle Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Chronicle, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Chronicle
provider_slug: chronicle
slug: chronicle-domain-security
source_filename: chronicle-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: chroniclehq.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  9 06:59:25 2026 GMT\n  hsts: true\n  hsts_max_age: 2592000\n- host: docs.chroniclehq.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 06:17:53 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.chroniclehq.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec  7 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: chroniclehq.com\n  dnssec: true\n  caa:\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/chronicle/refs/heads/main/security/chronicle-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Cloud Saas
- Presentations
- Artificial Intelligence
- Productivity
- Content Generation
- Agents
- MCP
- Developer API
---
