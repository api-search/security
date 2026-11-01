---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: offdeal.io
  spf: true
hosts:
- cert_expires: Jan  3 01:56:47 2027 GMT
  host: offdeal.io
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Offdeal Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for OffDeal, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: OffDeal
provider_slug: offdeal
slug: offdeal-domain-security
source_filename: offdeal-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: offdeal.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  3 01:56:47 2027 GMT\n  hsts: false\ndomains:\n- domain: offdeal.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/offdeal/security/offdeal-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- M&A
- InvestmentBank
- SmallBusiness
- Advisory
---
