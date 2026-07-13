---
description: ''
domains:
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
  domain: erxes.io
  spf: true
hosts:
- cert_expires: Oct  3 16:57:16 2026 GMT
  host: erxes.io
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Erxes Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Erxes, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Erxes
provider_slug: erxes
slug: erxes-domain-security
source_filename: erxes-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: erxes.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 16:57:16 2026 GMT\n  hsts: false\ndomains:\n- domain: erxes.io\n  dnssec: true\n  caa:\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/erxes/refs/heads/main/security/erxes-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- GraphQL
- CRM
- Customer Experience
- Open Source
- Marketing Automation
- Sales Pipeline
---
