---
description: ''
domains:
- caa:
  - 0 issuewild "digicert.com"
  - 0 issuewild "letsencrypt.org"
  - 0 issue "digicert.com"
  - 0 issue "godaddy.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "quovadisglobal.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: bis.org
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: fsb.org
  spf: true
hosts:
- cert_expires: Sep 18 01:04:45 2026 GMT
  host: www.bis.org
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 22 09:30:55 2026 GMT
  host: www.fsb.org
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 26 07:51:25 2026 GMT
  host: www.federalreserve.gov
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Banking Regulation Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Banking Regulation, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Banking Regulation
provider_slug: banking-regulation
slug: banking-regulation-domain-security
source_filename: banking-regulation-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.bis.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 18 01:04:45 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: www.fsb.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 22 09:30:55 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: www.federalreserve.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 26 07:51:25 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: bis.org\n  dnssec: false\n  caa:\n  - 0 issuewild \"digicert.com\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"godaddy.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"quovadisglobal.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: fsb.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/banking-regulation/refs/heads/main/security/banking-regulation-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- AML
- Banking
- Banking Regulation
- Basel
- Compliance
- Finance
- KYC
- RegTech
---
