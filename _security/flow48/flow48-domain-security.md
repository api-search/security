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
  dmarc_policy: reject
  dnssec: true
  domain: flow48.com
  spf: true
hosts:
- cert_expires: Sep 24 09:03:59 2026 GMT
  host: flow48.com
  hsts: true
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Flow48 Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Flow48, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Flow48
provider_slug: flow48
slug: flow48-domain-security
source_filename: flow48-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: flow48.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 24 09:03:59 2026 GMT\n  hsts: true\ndomains:\n- domain: flow48.com\n  dnssec: true\n  caa:\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"amazon.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/flow48/refs/heads/main/security/flow48-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Fintech
- Financial Services
- Embedded Finance
- SME Lending
- Revenue-Based Financing
- Invoice Financing
- MENA
- Speedinvest Portfolio
---
