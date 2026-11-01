---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: tourscanner.ai
  spf: true
hosts:
- cert_expires: Dec 26 19:06:25 2026 GMT
  host: tourscanner.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Tourscanner Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for TourScanner AI, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: TourScanner AI
provider_slug: tourscanner-ai
slug: tourscanner-ai-domain-security
source_filename: tourscanner-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: tourscanner.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 26 19:06:25 2026 GMT\n  hsts: false\ndomains:\n- domain: tourscanner.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/tourscanner-ai/security/tourscanner-ai-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Tours
- Activities
- API
- Booking
---
