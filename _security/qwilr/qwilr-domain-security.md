---
description: ''
domains:
- caa:
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "ssl.com"
  - 0 issuewild "amazon.com"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: qwilr.com
  spf: true
hosts:
- cert_expires: Sep 20 04:03:32 2026 GMT
  host: qwilr.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Qwilr Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Qwilr, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Qwilr
provider_slug: qwilr
slug: qwilr-domain-security
source_filename: qwilr-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: qwilr.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 20 04:03:32 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: qwilr.com\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"amazon.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/qwilr/refs/heads/main/security/qwilr-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Proposals
- Documents
- Sales
- Quotes
- Contracts
- E-Signature
- Webhooks
- MCP
- SaaS
---
