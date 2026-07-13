---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: ftc.gov
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: donotcall.gov
  spf: true
hosts:
- cert_expires: Feb  8 23:59:59 2027 GMT
  host: www.ftc.gov
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 16 15:21:19 2026 GMT
  host: api.ftc.gov
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- host: telemarketers.donotcall.gov
  https: false
kind: domain-security
layout: security
method: probed
name: Federal Trade Commission Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Federal Trade Commission, probed live across 3 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Federal Trade Commission
provider_slug: federal-trade-commission
slug: federal-trade-commission-domain-security
source_filename: federal-trade-commission-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.ftc.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  8 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.ftc.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 16 15:21:19 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: telemarketers.donotcall.gov\n  https: false\ndomains:\n- domain: ftc.gov\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: donotcall.gov\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/federal-trade-commission/refs/heads/main/security/federal-trade-commission-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Antitrust
- Consumer Protection
- Do Not Call
- Federal Government
- Law Enforcement
- Open Data
---
