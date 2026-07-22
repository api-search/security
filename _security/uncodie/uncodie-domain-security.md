---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: makinari.com
  spf: true
- caa:
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: uncodie.com
  spf: true
hosts:
- cert_expires: Oct  6 13:35:06 2026 GMT
  host: www.makinari.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  1 10:55:38 2026 GMT
  host: www.uncodie.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 10 23:44:51 2026 GMT
  host: docs.makinari.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Uncodie Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Uncodie (now Makinari), probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Uncodie (now Makinari)
provider_slug: uncodie
slug: uncodie-domain-security
source_filename: uncodie-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.makinari.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  6 13:35:06 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: www.uncodie.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 10:55:38 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.makinari.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 10 23:44:51 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: makinari.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: uncodie.com\n  dnssec: true\n  caa:\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  spf:\
  \ true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/uncodie/refs/heads/main/security/uncodie-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Artificial Intelligence
- AI Agents
- CRM
- Sales Automation
- Marketing Automation
- Lead Generation
- No Code
- MCP
---
