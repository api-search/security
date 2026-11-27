---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: aevia.cloud
  spf: true
hosts:
- cert_expires: Dec  3 16:11:44 2026 GMT
  host: aevia.cloud
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Aevia Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Aevia, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Aevia
provider_slug: aevia-cloud
slug: aevia-cloud-domain-security
source_filename: aevia-cloud-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: aevia.cloud\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  3 16:11:44 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: aevia.cloud\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/aevia-cloud/security/aevia-cloud-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
---
