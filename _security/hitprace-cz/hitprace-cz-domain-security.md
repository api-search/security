---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: hitprace.cz
  spf: true
hosts:
- cert_expires: Jan  8 16:03:30 2027 GMT
  host: hitprace.cz
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: TRAFFIC DRIVER s.r.o. Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for TRAFFIC DRIVER s.r.o., probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: TRAFFIC DRIVER s.r.o.
provider_slug: hitprace-cz
slug: hitprace-cz-domain-security
source_filename: hitprace-cz-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: hitprace.cz\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  8 16:03:30 2027 GMT\n  hsts: false\ndomains:\n- domain: hitprace.cz\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/hitprace-cz/security/hitprace-cz-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Job Portal
- Czech Republic
- Employment
- Careers
- Technology
---
