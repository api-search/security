---
description: ''
domains:
- caa:
  - 0 issue "digicert.com"
  - 0 issue "globalsign.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 issue "sectigo.com"
  - 0 issuewild "amazon.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: worldline.com
  spf: true
- caa:
  - 0 issue "amazontrust.com"
  - 0 issuewild "amazontrust.com"
  - 0 issue "sectigo.com"
  - 0 issuewild "sectigo.com"
  - 0 issue "swisssign.com"
  - 0 issuewild "swisssign.com"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: worldline-solutions.com
  spf: true
hosts:
- cert_expires: Dec 10 23:59:59 2026 GMT
  host: developer.worldline.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 10 23:59:59 2026 GMT
  host: worldline.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb 23 23:59:59 2027 GMT
  host: docs.connect.worldline-solutions.com
  hsts: true
  hsts_max_age: 3600
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Wordline Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Worldline, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Worldline
provider_slug: wordline
slug: wordline-domain-security
source_filename: wordline-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developer.worldline.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 10 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: worldline.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 10 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.connect.worldline-solutions.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Feb 23 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 3600\ndomains:\n- domain: worldline.com\n  dnssec: false\n  caa:\n  - 0 issue \"digicert.com\"\n  - 0 issue \"globalsign.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"sectigo.com\"\n  - 0 issuewild \"amazon.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: worldline-solutions.com\n  dnssec: false\n  caa:\n  - 0 issue \"amazontrust.com\"\n  - 0 issuewild \"amazontrust.com\"\
  \n  - 0 issue \"sectigo.com\"\n  - 0 issuewild \"sectigo.com\"\n  - 0 issue \"swisssign.com\"\n  - 0 issuewild \"swisssign.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wordline/refs/heads/main/security/wordline-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Payments
- Payment Processing
- Acquiring
- Issuing
- Open Banking
- Digital Banking
- FinTech
- Europe
---
