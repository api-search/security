---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: ifg.tax
  spf: true
hosts:
- cert_expires: Feb  1 10:04:12 2027 GMT
  host: ifg.tax
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: IFG Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for IFG, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: IFG
provider_slug: ifg-tax
slug: ifg-tax-domain-security
source_filename: ifg-tax-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ifg.tax\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  1 10:04:12 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: ifg.tax\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/ifg-tax/security/ifg-tax-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Tax
- Finance
- Legal
- Software-as-a-Service
---
