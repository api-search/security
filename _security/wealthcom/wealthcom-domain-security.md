---
description: ''
domains:
- caa:
  - 0 issue "amazonaws.com"
  - 0 issue "amazontrust.com"
  - 0 issue "awstrust.com"
  - 0 issue "digicert.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: wealth.com
  spf: true
hosts:
- cert_expires: Oct 11 09:16:47 2026 GMT
  host: www.wealth.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  6 05:13:03 2026 GMT
  host: developer.wealth.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Mar  3 23:59:59 2027 GMT
  host: advisor-api.wealth.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Wealthcom Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Wealth.com, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Wealth.com
provider_slug: wealthcom
slug: wealthcom-domain-security
source_filename: wealthcom-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.wealth.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 11 09:16:47 2026 GMT\n  hsts: false\n- host: developer.wealth.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  6 05:13:03 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: advisor-api.wealth.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar  3 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: wealth.com\n  dnssec: false\n  caa:\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"amazontrust.com\"\n  - 0 issue \"awstrust.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wealthcom/refs/heads/main/security/wealthcom-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Enterprise
- Estate Planning
- Tax Planning
- Wealth Management
- Financial Advisors
- Fintech
- Artificial Intelligence
---
