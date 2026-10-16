---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: circuity.com
  spf: true
hosts:
- cert_expires: Jan 18 14:06:49 2027 GMT
  host: circuity.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Circuity Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Circuity, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Circuity
provider_slug: circuity
slug: circuity-domain-security
source_filename: circuity-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-08'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: circuity.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 18 14:06:49 2027 GMT\n  hsts: false\ndomains:\n- domain: circuity.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/circuity/refs/heads/main/security/circuity-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Private-Market
- Equity
- Liquidity
- FinTech
---
