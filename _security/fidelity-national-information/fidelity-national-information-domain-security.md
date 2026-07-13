---
description: ''
domains:
- caa:
  - 0 issue "sectigo.com"
  - 0 issue "visa.com"
  - 0 issuewild "sectigo.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: fisglobal.com
  spf: true
hosts:
- cert_expires: Feb  9 23:59:59 2027 GMT
  host: www.fisglobal.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 24 23:59:59 2026 GMT
  host: codeconnect.fisglobal.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Fidelity National Information Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Fidelity National Information Services (FIS), probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Fidelity National Information Services (FIS)
provider_slug: fidelity-national-information
slug: fidelity-national-information-domain-security
source_filename: fidelity-national-information-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.fisglobal.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  9 23:59:59 2027 GMT\n  hsts: null\n- host: codeconnect.fisglobal.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 24 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: fisglobal.com\n  dnssec: false\n  caa:\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"visa.com\"\n  - 0 issuewild \"sectigo.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fidelity-national-information/refs/heads/main/security/fidelity-national-information-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Financial Services
- Payments
- Banking
- Capital Markets
- Wealth Management
- Risk and Compliance
- Fortune 500
---
