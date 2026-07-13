---
api_specs:
- filename: lex-machina-openapi.yml
  format: yaml
  label: Lex Machina Litigation Analytics API
  slug: lex-machina-litigation-analytics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lex-machina/refs/heads/main/openapi/lex-machina-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: lexisnexis.com
  spf: true
- caa:
  - 0 issue "amazontrust.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 issue "digicert.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: lexmachina.com
  spf: true
hosts:
- cert_expires: Apr 11 14:51:24 2027 GMT
  host: www.lexisnexis.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 18 16:29:49 2026 GMT
  host: developer.lexmachina.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  9 00:17:15 2026 GMT
  host: api.lexmachina.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Lex Machina Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Lex Machina, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Lex Machina
provider_slug: lex-machina
slug: lex-machina-domain-security
source_filename: lex-machina-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.lexisnexis.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Apr 11 14:51:24 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: developer.lexmachina.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 18 16:29:49 2026 GMT\n  hsts: false\n- host: api.lexmachina.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  9 00:17:15 2026 GMT\n  hsts: null\ndomains:\n- domain: lexisnexis.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: lexmachina.com\n  dnssec: false\n  caa:\n  - 0 issue \"amazontrust.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"digicert.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lex-machina/refs/heads/main/security/lex-machina-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Legal
- Legal Analytics
- Legal Technology
- Litigation
- Litigation Analytics
- Court Data
- Dockets
- Judges
- Law Firms
- Attorneys
- Patents
- PTAB
- ITC
- Bankruptcy
- Appeals
- State Courts
- Federal Courts
- LexisNexis
- Data
- Analytics
---
