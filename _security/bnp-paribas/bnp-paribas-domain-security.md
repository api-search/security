---
description: ''
domains:
- caa:
  - 0 iodef "mailto:report-abuse@globalsign.com"
  - 0 issue "globalsign.com"
  - 0 issue "d-trust.net"
  - 0 issue "pki.goog"
  - 0 issuewild ";"
  - 0 issue "digicert.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: bnpparibas.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: apistore.bnpparibas
  spf: true
hosts:
- cert_expires: Oct  5 23:59:59 2026 GMT
  host: www.bnpparibas.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 10 23:59:59 2026 GMT
  host: developers.cib.bnpparibas.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 18 23:59:59 2026 GMT
  host: apistore.bnpparibas
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Bnp Paribas Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for BNP Paribas, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: BNP Paribas
provider_slug: bnp-paribas
slug: bnp-paribas-domain-security
source_filename: bnp-paribas-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.bnpparibas.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  5 23:59:59 2026 GMT\n  hsts: null\n- host: developers.cib.bnpparibas.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 10 23:59:59 2026 GMT\n  hsts: false\n- host: apistore.bnpparibas\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 18 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: bnpparibas.com\n  dnssec: true\n  caa:\n  - 0 iodef \"mailto:report-abuse@globalsign.com\"\n  - 0 issue \"globalsign.com\"\n  - 0 issue \"d-trust.net\"\n  - 0 issue \"pki.goog\"\n  - 0 issuewild \";\"\n  - 0 issue \"digicert.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: apistore.bnpparibas\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bnp-paribas/refs/heads/main/security/bnp-paribas-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Banking
- Finance
- Payments
- Capital Markets
- Open Banking
---
