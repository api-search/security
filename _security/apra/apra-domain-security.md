---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: apra.gov.au
  spf: true
hosts:
- cert_expires: Oct 13 07:08:38 2026 GMT
  host: www.apra.gov.au
  hsts: true
  hsts_max_age: 31557600
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb 15 23:59:59 2027 GMT
  host: connect.apra.gov.au
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 15552000
  https: true
  note: APRA Connect production. F5 BIG-IP WAF answers anonymous requests with an HTTP 200 "Request Rejected" page. Highest negotiated protocol observed was TLSv1.2.
  tls_version: TLSv1.2
- cert_expires: Feb 15 23:59:59 2027 GMT
  host: connect-test.apra.gov.au
  hsts: false
  https: true
  note: APRA Connect test environment. Anonymous request returns HTTP/1.0 302 from BigIP; no Strict-Transport-Security header observed on that redirect.
  tls_version: TLSv1.2
- host: api.apra.gov.au
  https: false
  note: DNS A record 124.47.155.12 exists, but TCP/443 and TCP/80 both time out — no service is published on this name as of 2026-07-25. Recorded because the earlier review noted this name as non-resolving; it now resolves but does not answer.
kind: domain-security
layout: security
method: probed
name: Apra Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for APRA, probed live across 4 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: APRA
provider_slug: apra
slug: apra-domain-security
source_filename: apra-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-25'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml hosts (corporate site + APRA Connect\n  production/test + the unreachable api. name)\nhosts:\n- host: www.apra.gov.au\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 13 07:08:38 2026 GMT\n  hsts: true\n  hsts_max_age: 31557600\n- host: connect.apra.gov.au\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Feb 15 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 15552000\n  hsts_include_subdomains: true\n  note: APRA Connect production. F5 BIG-IP WAF answers anonymous requests with an HTTP\n    200 \"Request Rejected\" page. Highest negotiated protocol observed was TLSv1.2.\n- host: connect-test.apra.gov.au\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Feb 15 23:59:59 2027 GMT\n  hsts: false\n  note: APRA Connect test environment. Anonymous request returns HTTP/1.0 302 from\n    BigIP; no Strict-Transport-Security header observed on that redirect.\n- host: api.apra.gov.au\n\
  \  https: false\n  note: DNS A record 124.47.155.12 exists, but TCP/443 and TCP/80 both time out — no\n    service is published on this name as of 2026-07-25. Recorded because the earlier\n    review noted this name as non-resolving; it now resolves but does not answer.\ndomains:\n- domain: apra.gov.au\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/apra/refs/heads/main/security/apra-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Insurance
- Australia
- Regulator
- Prudential Regulation
- General Insurance
- Life Insurance
- Private Health Insurance
- Regulatory Reporting
- Market Infrastructure
- Risk Data
- Superannuation
- Banking
---
