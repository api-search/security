---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: orizn.app
  spf: true
hosts:
- cert_expires: Sep 10 05:10:16 2026 GMT
  host: visa.orizn.app
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Orizn Visa Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Orizn Visa, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Orizn Visa
provider_slug: orizn-visa
slug: orizn-visa-domain-security
source_filename: orizn-visa-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: visa.orizn.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 10 05:10:16 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: orizn.app\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/orizn-visa/refs/heads/main/security/orizn-visa-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Transportation
- Public APIs
---
