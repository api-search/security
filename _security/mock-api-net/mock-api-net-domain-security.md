---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: mock-api.net
  spf: true
hosts:
- cert_expires: Dec 13 10:15:52 2026 GMT
  host: mock-api.net
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Mock Api Net Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Prime Dev, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Prime Dev
provider_slug: mock-api-net
slug: mock-api-net-domain-security
source_filename: mock-api-net-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: mock-api.net\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec 13 10:15:52 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: mock-api.net\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/mock-api-net/security/mock-api-net-domain-security.yml
summary_line: TLSv1.2 · HSTS
tags:
- Company
---
