---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dns_aid:
    checked: '2026-11-26'
    published: false
  dnssec: true
  domain: taptax.co.uk
  spf: true
hosts:
- cert_expires: Jan 24 11:18:22 2027 GMT
  host: taptax.co.uk
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: TapTax Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for TapTax, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: TapTax
provider_slug: taptax-co-uk
slug: taptax-co-uk-domain-security
source_filename: taptax-co-uk-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: taptax.co.uk\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 24 11:18:22 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: taptax.co.uk\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n  dns_aid:\n    checked: '2026-11-26'\n    published: false\n"
source_yaml_url: https://artifacts.apis.io/taptax-co-uk/security/taptax-co-uk-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Tax
- MTD
- Accounting
- UK
- SaaS
---
