---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: biurko.io
  spf: true
hosts:
- cert_expires: Dec 23 17:07:52 2026 GMT
  host: biurko.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Biurko Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Biurko, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Biurko
provider_slug: biurko-io
slug: biurko-io-domain-security
source_filename: biurko-io-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: biurko.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 23 17:07:52 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: biurko.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/biurko-io/security/biurko-io-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Accounting
- Software-as-a-Service
- Poland
- Finance
- Invoicing
---
