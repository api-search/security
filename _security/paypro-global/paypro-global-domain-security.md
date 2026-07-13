---
description: ''
domains:
- caa:
  - 0 issue "pki.goog"
  - 0 issuewild "digicert.com"
  - 0 issue "digicert.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: payproglobal.com
  spf: true
hosts:
- cert_expires: Oct 25 23:59:59 2026 GMT
  host: payproglobal.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- host: developer.payproglobal.com
  https: false
kind: domain-security
layout: security
method: probed
name: Paypro Global Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for PayPro Global, probed live across 2 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: PayPro Global
provider_slug: paypro-global
slug: paypro-global-domain-security
source_filename: paypro-global-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: payproglobal.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 25 23:59:59 2026 GMT\n  hsts: false\n- host: developer.payproglobal.com\n  https: false\ndomains:\n- domain: payproglobal.com\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  - 0 issuewild \"digicert.com\"\n  - 0 issue \"digicert.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/paypro-global/refs/heads/main/security/paypro-global-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- E-Commerce
- Merchant of Record
- Payments
- SaaS
- Subscription Billing
- Tax Compliance
---
