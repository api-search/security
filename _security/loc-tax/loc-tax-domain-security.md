---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: loc.tax
  spf: true
hosts:
- cert_expires: Jan  7 05:10:26 2027 GMT
  host: www.loc.tax
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Loc Tax Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Loctax, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Loctax
provider_slug: loc-tax
slug: loc-tax-domain-security
source_filename: loc-tax-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-25'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.loc.tax\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  7 05:10:26 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: loc.tax\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/loc-tax/security/loc-tax-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Tax
- AI
- Platform
- Global
- Compliance
---
