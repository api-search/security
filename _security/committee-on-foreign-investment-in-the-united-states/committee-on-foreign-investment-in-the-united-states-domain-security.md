---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: treasury.gov
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: ecfr.gov
  spf: true
hosts:
- cert_expires: Sep 23 21:25:47 2026 GMT
  host: home.treasury.gov
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 24 23:59:59 2026 GMT
  host: www.ecfr.gov
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Committee On Foreign Investment In The United States Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Committee on Foreign Investment in the United States, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Committee on Foreign Investment in the United States
provider_slug: committee-on-foreign-investment-in-the-united-states
slug: committee-on-foreign-investment-in-the-united-states-domain-security
source_filename: committee-on-foreign-investment-in-the-united-states-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: home.treasury.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 23 21:25:47 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: www.ecfr.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 24 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: treasury.gov\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: ecfr.gov\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/committee-on-foreign-investment-in-the-united-states/refs/heads/main/security/committee-on-foreign-investment-in-the-united-states-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- CFIUS
- Federal Government
- Foreign Investment
- National Security
- Regulation
- Treasury
---
