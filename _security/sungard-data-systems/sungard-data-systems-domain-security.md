---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: sungard-data-systems.com
  spf: false
- caa:
  - 0 issue "visa.com"
  - 0 issuewild "sectigo.com"
  - 0 issue "sectigo.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: fisglobal.com
  spf: true
hosts:
- host: www.sungard-data-systems.com
  https: false
- cert_expires: Feb  9 23:59:59 2027 GMT
  host: www.fisglobal.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Sungard Data Systems Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for SunGard Data Systems, probed live across 2 host(s) and 2 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: SunGard Data Systems
provider_slug: sungard-data-systems
slug: sungard-data-systems-domain-security
source_filename: sungard-data-systems-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.sungard-data-systems.com\n  https: false\n- host: www.fisglobal.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  9 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: sungard-data-systems.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n- domain: fisglobal.com\n  dnssec: false\n  caa:\n  - 0 issue \"visa.com\"\n  - 0 issuewild \"sectigo.com\"\n  - 0 issue \"sectigo.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sungard-data-systems/refs/heads/main/security/sungard-data-systems-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Financial Services
- Capital Markets
- Risk Management
- Treasury
- Enterprise Software
- Acquired
- Fortune 1000
---
