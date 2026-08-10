---
description: ''
domains:
- caa:
  - 0 issuewild "godaddy.com"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "sectigo.com"
  - 0 issuewild "ssl.com"
  - 0 issue "comodoca.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: brightplan.com
  spf: true
hosts:
- cert_expires: Nov 23 16:22:53 2026 GMT
  host: www.brightplan.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 23 16:22:53 2026 GMT
  host: my.brightplan.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  note: employee-facing application host; single-page app that answers HTTP 200 with the same HTML shell for every path
  tls_version: TLSv1.3
- cert_expires: Nov 23 16:22:53 2026 GMT
  host: web.brightplan.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  note: application host my.brightplan.com/login redirects to
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Brightplan Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for BrightPlan, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: BrightPlan
provider_slug: brightplan
slug: brightplan-domain-security
source_filename: brightplan-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-08'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.brightplan.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 23 16:22:53 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: my.brightplan.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 23 16:22:53 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\n  note: employee-facing application host; single-page app that answers HTTP 200 with\n    the same HTML shell for every path\n- host: web.brightplan.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 23 16:22:53 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\n  note: application host my.brightplan.com/login redirects to\ndomains:\n- domain: brightplan.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"godaddy.com\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"sectigo.com\"\n  - 0 issuewild \"ssl.com\"\
  \n  - 0 issue \"comodoca.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/brightplan/refs/heads/main/security/brightplan-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Financial Wellness
- Financial Planning
- Employee Benefits
- Human Resources
- Wealth Management
- Financial Services
- Retirement
- Investment Advice
- Company
---
