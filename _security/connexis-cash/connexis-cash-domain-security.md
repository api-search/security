---
description: ''
domains:
- caa:
  - 0 issue "d-trust.net"
  - 0 iodef "mailto:report-abuse@globalsign.com"
  - 0 issuewild ";"
  - 0 issue "globalsign.com"
  - 0 issue "entrust.net"
  - 0 issue "digicert.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: bnpparibas.com
  spf: true
hosts:
- cert_expires: Sep  2 23:59:59 2026 GMT
  host: cashmanagement.bnpparibas.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 10 23:59:59 2026 GMT
  host: developers.cib.bnpparibas.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb 10 23:59:59 2027 GMT
  host: psd2.api.cib.bnpparibas.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Connexis Cash Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Connexis Cash, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Connexis Cash
provider_slug: connexis-cash
slug: connexis-cash-domain-security
source_filename: connexis-cash-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: cashmanagement.bnpparibas.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  2 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developers.cib.bnpparibas.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 10 23:59:59 2026 GMT\n  hsts: false\n- host: psd2.api.cib.bnpparibas.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 10 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: bnpparibas.com\n  dnssec: true\n  caa:\n  - 0 issue \"d-trust.net\"\n  - 0 iodef \"mailto:report-abuse@globalsign.com\"\n  - 0 issuewild \";\"\n  - 0 issue \"globalsign.com\"\n  - 0 issue \"entrust.net\"\n  - 0 issue \"digicert.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/connexis-cash/refs/heads/main/security/connexis-cash-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Account Information
- BNP Paribas
- Cash Management
- Corporate Banking
- Digital Banking
- Liquidity Management
- Open Banking
- Payments
- PSD2
- SCA
- STET
---
