---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: raymondjames.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: rjf.com
  spf: true
hosts:
- cert_expires: Sep 12 23:59:59 2026 GMT
  host: www.raymondjames.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 10 23:59:59 2026 GMT
  host: clientaccess.rjf.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Raymond James Financial Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Raymond James Financial, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Raymond James Financial
provider_slug: raymond-james-financial
slug: raymond-james-financial-domain-security
source_filename: raymond-james-financial-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.raymondjames.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 12 23:59:59 2026 GMT\n  hsts: null\n- host: clientaccess.rjf.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 10 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: raymondjames.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: rjf.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/raymond-james-financial/refs/heads/main/security/raymond-james-financial-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Asset Management
- Banking
- Brokerage
- Capital Markets
- Financial Services
- Fortune 500
- Investment Banking
- Investment Management
- Wealth Management
---
