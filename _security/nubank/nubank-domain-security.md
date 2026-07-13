---
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 issue "sectigo.com"
  - 0 issuewild "amazon.com"
  - 0 issuewild "globalsign.com"
  - 0 issuewild "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: nubank.com.br
  spf: true
- caa: []
  dmarc: false
  dnssec: true
  domain: dev.br
  spf: false
hosts:
- cert_expires: Jan 17 23:59:59 2027 GMT
  host: nubank.com.br
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- host: openfinance.dev.br
  hsts: null
  https: true
  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: certificate has expired (_ssl.c:1082)'
- host: openbanking.nubank.com.br
  https: false
kind: domain-security
layout: security
method: probed
name: Nubank Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Nu (Nubank), probed live across 3 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Nu (Nubank)
provider_slug: nubank
slug: nubank-domain-security
source_filename: nubank-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: nubank.com.br\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 17 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: openfinance.dev.br\n  https: true\n  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: certificate has\n    expired (_ssl.c:1082)'\n  hsts: null\n- host: openbanking.nubank.com.br\n  https: false\ndomains:\n- domain: nubank.com.br\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"sectigo.com\"\n  - 0 issuewild \"amazon.com\"\n  - 0 issuewild \"globalsign.com\"\n  - 0 issuewild \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: dev.br\n  dnssec: true\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nubank/refs/heads/main/security/nubank-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Neobank
- Banking
- Credit Cards
- Open Finance
- Payments
- Brazil
- Mexico
- Colombia
- Latin America
---
