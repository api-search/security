---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: divvydiary.com
  spf: true
hosts:
- cert_expires: Jan 10 20:51:37 2027 GMT
  host: divvydiary.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Divvydiary Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for DivvyDiary, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: DivvyDiary
provider_slug: divvydiary
slug: divvydiary-domain-security
source_filename: divvydiary-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-27'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: divvydiary.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 10 20:51:37 2027 GMT\n  hsts: false\ndomains:\n- domain: divvydiary.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/divvydiary/security/divvydiary-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Finance
- Investment
- Dividend
- Portfolio
---
