---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: centurylink.com
  spf: true
- caa:
  - 0 issue "amazon.com"
  - 0 issue "globalsign.com"
  - 0 issuewild "digicert.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "digicert.com"
  - 0 issuewild "globalsign.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: lumen.com
  spf: true
hosts:
- cert_expires: Mar  2 23:59:59 2027 GMT
  host: www.centurylink.com
  hsts: true
  hsts_max_age: 157680000
  https: true
  tls_version: TLSv1.2
- cert_expires: Jan  5 23:59:59 2027 GMT
  host: developer.lumen.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- host: apimarketplace.lumen.com
  hsts: null
  https: true
  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: certificate has expired (_ssl.c:1082)'
kind: domain-security
layout: security
method: probed
name: Centurylink Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for CenturyLink (Lumen Technologies), probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: CenturyLink (Lumen Technologies)
provider_slug: centurylink
slug: centurylink-domain-security
source_filename: centurylink-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.centurylink.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Mar  2 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 157680000\n- host: developer.lumen.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  5 23:59:59 2027 GMT\n  hsts: false\n- host: apimarketplace.lumen.com\n  https: true\n  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: certificate has\n    expired (_ssl.c:1082)'\n  hsts: null\ndomains:\n- domain: centurylink.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: lumen.com\n  dnssec: false\n  caa:\n  - 0 issue \"amazon.com\"\n  - 0 issue \"globalsign.com\"\n  - 0 issuewild \"digicert.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"digicert.com\"\n  - 0 issuewild \"globalsign.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/centurylink/refs/heads/main/security/centurylink-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Broadband
- Connectivity
- Edge
- Fiber
- Lumen
- Network
- OAuth 2.0
- Quantum Fiber
- SD-WAN
- Telecom
- Fortune 500
---
