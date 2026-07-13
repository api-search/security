---
description: ''
domains:
- caa:
  - 0 issuewild "amazon.com"
  - 0 issue "amazon.com"
  - 0 issuewild "digicert.com"
  - 0 issue "digicert.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: quicken.com
  spf: true
- caa:
  - 0 issue "amazon.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "digicert.com"
  - 0 issuewild "amazon.com"
  - 0 issuewild "digicert.com"
  dmarc: false
  dnssec: false
  domain: simplifimoney.com
  spf: false
hosts:
- cert_expires: Aug 16 23:59:59 2026 GMT
  host: www.quicken.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jul 17 23:59:59 2026 GMT
  host: app.simplifimoney.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Simplifi Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Simplifi by Quicken, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Simplifi by Quicken
provider_slug: simplifi
slug: simplifi-domain-security
source_filename: simplifi-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.quicken.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 16 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: app.simplifimoney.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jul 17 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: quicken.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"amazon.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issuewild \"digicert.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: simplifimoney.com\n  dnssec: false\n  caa:\n  - 0 issue \"amazon.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"digicert.com\"\n  - 0 issuewild \"amazon.com\"\n  - 0 issuewild \"digicert.com\"\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/simplifi/refs/heads/main/security/simplifi-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Personal Finance
- Budgeting
- Financial Aggregation
- Account Management
- Spending Tracking
- Investment Tracking
- Savings Goals
- Cash Flow
---
