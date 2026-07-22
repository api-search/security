---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: faqtor.io
  spf: false
hosts:
- cert_expires: Sep 27 18:15:12 2026 GMT
  host: faqtor.io
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Faqtor Inc Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Faqtor, Inc., probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Faqtor, Inc.
provider_slug: faqtor-inc
slug: faqtor-inc-domain-security
source_filename: faqtor-inc-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: faqtor.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 27 18:15:12 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: faqtor.io\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/faqtor-inc/refs/heads/main/security/faqtor-inc-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
---
