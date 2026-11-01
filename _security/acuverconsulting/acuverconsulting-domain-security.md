---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: acuverconsulting.com
  spf: true
hosts:
- cert_expires: Nov 29 09:03:42 2026 GMT
  host: acuverconsulting.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Acuverconsulting Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Acuver consulting, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Acuver consulting
provider_slug: acuverconsulting
slug: acuverconsulting-domain-security
source_filename: acuverconsulting-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: acuverconsulting.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 29 09:03:42 2026 GMT\n  hsts: false\ndomains:\n- domain: acuverconsulting.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/acuverconsulting/security/acuverconsulting-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Consulting
- Supply Chain
- Technology
- Services
- Software
---
