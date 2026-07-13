---
description: ''
domains:
- caa:
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "sectigo.com"
  - 0 issuewild "ssl.com"
  - 0 iodef "mailto:devops@m1finance.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: m1.com
  spf: true
hosts:
- cert_expires: Aug 23 00:16:00 2026 GMT
  host: m1.com
  hsts: true
  hsts_max_age: 31536001
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: M1 Finance Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for M1 Finance, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: M1 Finance
provider_slug: m1-finance
slug: m1-finance-domain-security
source_filename: m1-finance-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: m1.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 23 00:16:00 2026 GMT\n  hsts: true\n  hsts_max_age: 31536001\ndomains:\n- domain: m1.com\n  dnssec: true\n  caa:\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"sectigo.com\"\n  - 0 issuewild \"ssl.com\"\n  - 0 iodef \"mailto:devops@m1finance.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/m1-finance/refs/heads/main/security/m1-finance-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Investing
- Fintech
- Fractional Shares
- Portfolio Management
- Robo-Advisor
- Margin Loans
- Banking
- Automated Investing
- Finance Super App
- Wealth Management
---
