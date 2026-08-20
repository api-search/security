---
description: ''
domains:
- caa:
  - 0 issuewild "ssl.com"
  - 0 issuewild "entrust.net"
  - 0 issue "letsencrypt.org"
  - 0 issuewild "digicert.com"
  - 0 issue "digicert.com"
  - 0 issuewild "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: intactfc.com
  spf: true
- caa:
  - 0 issue "digicert.com"
  - 0 issuewild "sectigo.com"
  - 0 issuewild "ssl.com"
  - 0 issuewild "entrust.net"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "amazon.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: intact.ca
  spf: true
hosts:
- cert_expires: Nov 27 23:59:59 2026 GMT
  host: www.intactfc.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 22 23:59:59 2026 GMT
  host: www.intact.ca
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec  4 23:59:59 2026 GMT
  host: www.intactspecialty.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Intact Financial Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Intact Financial, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Intact Financial
provider_slug: intact-financial
slug: intact-financial-domain-security
source_filename: intact-financial-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-25'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.intactfc.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 27 23:59:59 2026 GMT\n  hsts: null\n- host: www.intact.ca\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 22 23:59:59 2026 GMT\n  hsts: null\n- host: www.intactspecialty.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  4 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: intactfc.com\n  dnssec: true\n  caa:\n  - 0 issuewild \"ssl.com\"\n  - 0 issuewild \"entrust.net\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issuewild \"digicert.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issuewild \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: intact.ca\n  dnssec: true\n  caa:\n  - 0 issue \"digicert.com\"\n  - 0 issuewild \"sectigo.com\"\n  - 0 issuewild \"ssl.com\"\n  - 0 issuewild \"entrust.net\"\n  - 0 issuewild \"letsencrypt.org\"\
  \n  - 0 issuewild \"amazon.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/intact-financial/refs/heads/main/security/intact-financial-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Insurance
- Canada
- Property and Casualty
- Carrier
- Underwriting
- Claims
- Brokers
- Partner Gated
- No Public API
- CSIO
---
