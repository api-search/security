---
description: ''
domains:
- caa:
  - 0 issuewild "identrust.com"
  - 0 iodef "mailto:certnotification@thehartford.com"
  - 0 issue "digicert.com"
  - 0 issuewild "digicert.com"
  - 0 issue "identrust.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: thehartford.com
  spf: true
hosts:
- cert_expires: Sep 13 23:59:59 2026 GMT
  host: www.thehartford.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Hartford Financial Services Group Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Hartford Financial Services Group, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Hartford Financial Services Group
provider_slug: hartford-financial-services-group
slug: hartford-financial-services-group-domain-security
source_filename: hartford-financial-services-group-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.thehartford.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 13 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: thehartford.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"identrust.com\"\n  - 0 iodef \"mailto:certnotification@thehartford.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issuewild \"digicert.com\"\n  - 0 issue \"identrust.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hartford-financial-services-group/refs/heads/main/security/hartford-financial-services-group-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Fortune 500
- Insurance
- Property and Casualty
- Group Benefits
- Mutual Funds
- Financial Services
---
