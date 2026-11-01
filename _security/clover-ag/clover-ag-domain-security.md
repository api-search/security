---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: clover.ag
  spf: true
hosts:
- cert_expires: Nov  4 22:38:18 2026 GMT
  host: www.clover.ag
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Clover Ag Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Deep Rooted, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Deep Rooted
provider_slug: clover-ag
slug: clover-ag-domain-security
source_filename: clover-ag-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.clover.ag\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  4 22:38:18 2026 GMT\n  hsts: false\ndomains:\n- domain: clover.ag\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/clover-ag/security/clover-ag-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
---
