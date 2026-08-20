---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: usitc.gov
  spf: true
hosts:
- cert_expires: Aug 24 17:50:11 2026 GMT
  host: www.usitc.gov
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 24 17:50:11 2026 GMT
  host: dataweb.usitc.gov
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: International Trade Commission Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for International Trade Commission, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: International Trade Commission
provider_slug: international-trade-commission
slug: international-trade-commission-domain-security
source_filename: international-trade-commission-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.usitc.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 24 17:50:11 2026 GMT\n  hsts: null\n- host: dataweb.usitc.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 24 17:50:11 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: usitc.gov\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/international-trade-commission/refs/heads/main/security/international-trade-commission-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Federal-Government
- Government Data
- Intellectual Property
- Trade
- Tariffs
---
