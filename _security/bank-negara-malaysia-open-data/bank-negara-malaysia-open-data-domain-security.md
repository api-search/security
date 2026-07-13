---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: bnm.gov.my
  spf: true
hosts:
- cert_expires: Nov 26 23:59:59 2026 GMT
  host: apikijangportal.bnm.gov.my
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Bank Negara Malaysia Open Data Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Bank Negara Malaysia Open Data, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Bank Negara Malaysia Open Data
provider_slug: bank-negara-malaysia-open-data
slug: bank-negara-malaysia-open-data-domain-security
source_filename: bank-negara-malaysia-open-data-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: apikijangportal.bnm.gov.my\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 26 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: bnm.gov.my\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bank-negara-malaysia-open-data/refs/heads/main/security/bank-negara-malaysia-open-data-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Government
- Public APIs
---
