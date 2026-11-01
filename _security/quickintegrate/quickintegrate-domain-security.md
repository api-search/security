---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: quickintegrate.io
  spf: true
hosts:
- cert_expires: Dec  4 13:20:09 2026 GMT
  host: quickintegrate.io
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Quickintegrate Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ATDEV Services, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: ATDEV Services
provider_slug: quickintegrate
slug: quickintegrate-domain-security
source_filename: quickintegrate-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: quickintegrate.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  4 13:20:09 2026 GMT\n  hsts: null\ndomains:\n- domain: quickintegrate.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/quickintegrate/security/quickintegrate-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
---
