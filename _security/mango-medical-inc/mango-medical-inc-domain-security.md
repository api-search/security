---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: mangomedical.io
  spf: true
hosts:
- cert_expires: Oct 18 06:04:46 2026 GMT
  host: mangomedical.io
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Mango Medical Inc Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Mango Medical Inc, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Mango Medical Inc
provider_slug: mango-medical-inc
slug: mango-medical-inc-domain-security
source_filename: mango-medical-inc-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: mangomedical.io\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct 18 06:04:46 2026 GMT\n  hsts: null\ndomains:\n- domain: mangomedical.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mango-medical-inc/refs/heads/main/security/mango-medical-inc-domain-security.yml
summary_line: TLSv1.2
tags:
- Company
- Healthcare
- Medical
- Startup
- Y Combinator
---
