---
description: ''
domains:
- caa:
  - 0 issue "godaddy.com"
  - 0 issue "digicert.com"
  - 0 issue "entrust.net"
  - 0 issue "globalsign.com"
  - 0 issue "letsencrypt.org"
  - 0 iodef "mailto:webmaster@vancity.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: vancitycommunityinvestmentbank.ca
  spf: true
hosts:
- cert_expires: Sep 18 20:58:41 2026 GMT
  host: www.vancitycommunityinvestmentbank.ca
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Vancity Community Investment Bank Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Vancity Community Investment Bank, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Vancity Community Investment Bank
provider_slug: vancity-community-investment-bank
slug: vancity-community-investment-bank-domain-security
source_filename: vancity-community-investment-bank-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-23'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.vancitycommunityinvestmentbank.ca\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 18 20:58:41 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: vancitycommunityinvestmentbank.ca\n  dnssec: false\n  caa:\n  - 0 issue \"godaddy.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"entrust.net\"\n  - 0 issue \"globalsign.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 iodef \"mailto:webmaster@vancity.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vancity-community-investment-bank/refs/heads/main/security/vancity-community-investment-bank-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Financial-Services
- Banking
- Canada
- Schedule I Bank
- Credit Union
- Impact Banking
- Community Finance
- Consumer-Driven Banking
---
