---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: thesis.co
  spf: true
hosts:
- cert_expires: Jan 26 16:04:49 2027 GMT
  host: thesis.co
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Thesis Co Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Thesis, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Thesis
provider_slug: thesis-co
slug: thesis-co-domain-security
source_filename: thesis-co-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: thesis.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 26 16:04:49 2027 GMT\n  hsts: false\ndomains:\n- domain: thesis.co\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/thesis-co/security/thesis-co-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- venture studio
- Bitcoin
- decentralized products
- crypto
- blockchain
---
