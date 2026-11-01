---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: artificl.us
  spf: true
hosts:
- cert_expires: Dec 22 06:47:22 2026 GMT
  host: artificl.us
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Artificl Us Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for artificl-us, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: artificl-us
provider_slug: artificl-us
slug: artificl-us-domain-security
source_filename: artificl-us-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: artificl.us\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 22 06:47:22 2026 GMT\n  hsts: false\ndomains:\n- domain: artificl.us\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/artificl-us/security/artificl-us-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Compliance
- AI
- Document Tracking
- Small Business
---
