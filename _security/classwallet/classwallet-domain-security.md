---
description: ''
domains:
- caa:
  - 0 iodef "mailto:security@classwallet.com"
  - 0 issue "amazon.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 issuewild "amazon.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: classwallet.com
  spf: true
hosts:
- cert_expires: Aug 31 01:41:42 2026 GMT
  host: classwallet.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Classwallet Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ClassWallet, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: ClassWallet
provider_slug: classwallet
slug: classwallet-domain-security
source_filename: classwallet-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: classwallet.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 31 01:41:42 2026 GMT\n  hsts: false\ndomains:\n- domain: classwallet.com\n  dnssec: true\n  caa:\n  - 0 iodef \"mailto:security@classwallet.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 issuewild \"amazon.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/classwallet/refs/heads/main/security/classwallet-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
- Fintech
- Payments
- Digital Wallet
- Fund Management
- Education
- EdTech
- Government
- Compliance
---
