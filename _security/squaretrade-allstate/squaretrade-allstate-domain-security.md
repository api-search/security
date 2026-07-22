---
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "entrust.net"
  - 0 issue "amazon.com"
  - 0 issue "digicert.com"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: squaretrade.com
  spf: true
hosts:
- cert_expires: Jan 22 23:59:59 2027 GMT
  host: www.squaretrade.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Squaretrade Allstate Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for SquareTrade (Allstate), probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: SquareTrade (Allstate)
provider_slug: squaretrade-allstate
slug: squaretrade-allstate-domain-security
source_filename: squaretrade-allstate-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.squaretrade.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 22 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: squaretrade.com\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"entrust.net\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"digicert.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/squaretrade-allstate/refs/heads/main/security/squaretrade-allstate-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Fintech
- Insurance
- Warranty
- Product Protection
- Extended Warranty
- Consumer Electronics
- Claims
---
