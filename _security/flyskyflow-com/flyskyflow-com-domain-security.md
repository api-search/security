---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: flyskyflow.com
  spf: true
hosts:
- cert_expires: Nov 23 10:47:11 2026 GMT
  host: flyskyflow.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Flyskyflow Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Skyflow, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Skyflow
provider_slug: flyskyflow-com
slug: flyskyflow-com-domain-security
source_filename: flyskyflow-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-23'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: flyskyflow.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 23 10:47:11 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: flyskyflow.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/flyskyflow-com/security/flyskyflow-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
---
