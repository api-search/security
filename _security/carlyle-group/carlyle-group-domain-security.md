---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: carlyle.com
  spf: true
hosts:
- cert_expires: Aug 21 20:47:41 2026 GMT
  host: www.carlyle.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 19 23:59:59 2026 GMT
  host: lpconnect.carlyle.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  6 04:57:24 2026 GMT
  host: directlending.carlyle.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Carlyle Group Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for The Carlyle Group, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: The Carlyle Group
provider_slug: carlyle-group
slug: carlyle-group-domain-security
source_filename: carlyle-group-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.carlyle.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 21 20:47:41 2026 GMT\n  hsts: null\n- host: lpconnect.carlyle.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 19 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: directlending.carlyle.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  6 04:57:24 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: carlyle.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/carlyle-group/refs/heads/main/security/carlyle-group-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Alternative Assets
- Asset Management
- Direct Lending
- Global Credit
- Investment Firm
- Investor Portal
- Limited Partners
- Private Credit
- Private Equity
- Real Assets
- Fortune 1000
---
