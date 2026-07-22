---
description: ''
domains:
- caa:
  - 0 iodef "mailto:security@renofi.com"
  - 0 issue "certainly.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: renofi.com
  spf: true
hosts:
- cert_expires: Aug 30 21:44:54 2026 GMT
  host: www.renofi.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Renofi Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for RenoFi, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: RenoFi
provider_slug: renofi
slug: renofi-domain-security
source_filename: renofi-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.renofi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 30 21:44:54 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: renofi.com\n  dnssec: true\n  caa:\n  - 0 iodef \"mailto:security@renofi.com\"\n  - 0 issue \"certainly.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/renofi/refs/heads/main/security/renofi-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Fintech
- Lending
- Home Improvement
- Real Estate
- Mortgage
- Home Equity
- Renovation Financing
---
