---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: cozen.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: copublicstrategies.com
  spf: false
hosts:
- cert_expires: Dec  4 23:59:59 2026 GMT
  host: www.cozen.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 17 15:24:48 2026 GMT
  host: www.copublicstrategies.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Cozen Oconnor Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cozen O''Connor, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Cozen O'Connor
provider_slug: cozen-oconnor
slug: cozen-oconnor-domain-security
source_filename: cozen-oconnor-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.cozen.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  4 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: www.copublicstrategies.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 17 15:24:48 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: cozen.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: copublicstrategies.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cozen-oconnor/refs/heads/main/security/cozen-oconnor-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Am Law 100
- Corporate Law
- Government Affairs
- Insurance Law
- Intellectual Property
- Labor And Employment
- Law
- Law Firm
- Legal Services
- Litigation
- Lobbying
- Professional Services
- Public Strategies
- Real Estate
- Subrogation
- Thought Leadership
---
