---
description: ''
domains:
- caa:
  - 0 issue "amazontrust.com"
  - 0 issue "comodo.com"
  - 0 issue "digicert.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 issuewild "digicert.com"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: wealthfront.com
  spf: true
hosts:
- cert_expires: Dec 14 23:59:59 2026 GMT
  host: www.wealthfront.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 24 23:46:31 2026 GMT
  host: support.wealthfront.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Wealthfront Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Wealthfront, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Wealthfront
provider_slug: wealthfront
slug: wealthfront-domain-security
source_filename: wealthfront-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.wealthfront.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 14 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: support.wealthfront.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 24 23:46:31 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: wealthfront.com\n  dnssec: false\n  caa:\n  - 0 issue \"amazontrust.com\"\n  - 0 issue \"comodo.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 issuewild \"digicert.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wealthfront/refs/heads/main/security/wealthfront-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Finance
- Investment
- Portfolio Management
- Tax Optimization
- Robo-Advisor
- Wealth Management
- Cash Management
- Direct Indexing
- Financial Planning
- FinTech
---
