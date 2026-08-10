---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: splashfinancial.com
  spf: true
hosts:
- cert_expires: Oct 16 10:53:26 2026 GMT
  host: www.splashfinancial.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Splash Financial Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Splash Financial, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Splash Financial
provider_slug: splash-financial
slug: splash-financial-domain-security
source_filename: splash-financial-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.splashfinancial.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 16 10:53:26 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: splashfinancial.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/splash-financial/refs/heads/main/security/splash-financial-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Financial Services
- Lending
- Student Loans
- Personal Loans
- Marketplace
- Fintech
- Debt Consolidation
- Home Equity
---
