---
description: ''
domains:
- caa:
  - 0 issue "awstrust.com"
  - 0 issue "digicert.com"
  - 0 issue "godaddy.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "amazon.com"
  - 0 issue "amazontrust.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: debtbook.com
  spf: true
hosts:
- cert_expires: Sep 28 14:28:11 2026 GMT
  host: www.debtbook.com
  hsts: null
  https: true
  note: marketing site served by HubSpot CMS; no Strict-Transport-Security header observed
  tls_version: TLSv1.3
- cert_expires: Jan 29 23:59:59 2027 GMT
  host: app.debtbook.com
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 31536000
  https: true
  note: production application host (in scope for the vulnerability disclosure program)
  tls_version: TLSv1.3
- cert_expires: Sep 14 15:23:58 2026 GMT
  host: status.debtbook.com
  hsts: true
  hsts_max_age: 259200
  https: true
  note: Atlassian Statuspage
  tls_version: TLSv1.3
- cert_expires: Sep 14 13:34:31 2026 GMT
  host: trust.debtbook.com
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 31536000
  hsts_preload: true
  https: true
  note: SecurityPal-hosted trust center
  tls_version: TLSv1.3
- cert_expires: Dec 15 23:59:59 2026 GMT
  host: support.debtbook.com
  hsts: null
  https: true
  note: Intercom-hosted help center; redirects (302) to /en/
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Debtbook Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for DebtBook, probed live across 5 host(s) and 1 registrable domain(s). 5 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: DebtBook
provider_slug: debtbook
slug: debtbook-domain-security
source_filename: debtbook-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.debtbook.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 28 14:28:11 2026 GMT\n  hsts: null\n  note: marketing site served by HubSpot CMS; no Strict-Transport-Security header observed\n- host: app.debtbook.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 29 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n  hsts_include_subdomains: true\n  note: production application host (in scope for the vulnerability disclosure program)\n- host: status.debtbook.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 15:23:58 2026 GMT\n  hsts: true\n  hsts_max_age: 259200\n  note: Atlassian Statuspage\n- host: trust.debtbook.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 13:34:31 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n  hsts_include_subdomains: true\n  hsts_preload: true\n  note: SecurityPal-hosted\
  \ trust center\n- host: support.debtbook.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 15 23:59:59 2026 GMT\n  hsts: null\n  note: Intercom-hosted help center; redirects (302) to /en/\ndomains:\n- domain: debtbook.com\n  dnssec: true\n  caa:\n  - 0 issue \"awstrust.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"godaddy.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"amazontrust.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/debtbook/refs/heads/main/security/debtbook-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Treasury Management
- Government
- Public Finance
- Debt Management
- Cash Management
- Accounting
- Lease Accounting
- Investment Management
- Non-Profit
- Higher Education
- Healthcare
- Software-as-a-Service
---
