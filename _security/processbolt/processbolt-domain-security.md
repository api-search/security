---
description: ''
domains:
- caa:
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  - 0 issue "amazon.com"
  - 0 issue "awstrust.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: perimeter.net
  spf: true
hosts:
- cert_expires: Sep 17 21:56:19 2026 GMT
  host: perimeter.net
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Processbolt Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Perimeter VRM (formerly ProcessBolt), probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Perimeter VRM (formerly ProcessBolt)
provider_slug: processbolt
slug: processbolt-domain-security
source_filename: processbolt-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: perimeter.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 17 21:56:19 2026 GMT\n  hsts: false\ndomains:\n- domain: perimeter.net\n  dnssec: false\n  caa:\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"awstrust.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/processbolt/refs/heads/main/security/processbolt-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Vendor Risk Management
- Third-Party Risk
- Governance Risk Compliance
- Cybersecurity
- Risk Assessment
- Security
- Attack Surface Management
---
