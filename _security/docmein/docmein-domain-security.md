---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: docmein.com
  spf: true
hosts:
- cert_expires: Jan 15 16:33:54 2027 GMT
  host: www.docmein.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Docmein Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Docmein, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Docmein
provider_slug: docmein
slug: docmein-domain-security
source_filename: docmein-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-23'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.docmein.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 15 16:33:54 2027 GMT\n  hsts: false\ndomains:\n- domain: docmein.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/docmein/security/docmein-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
- Healthcare
- Scheduling
- Software-as-a-Service
- Free
---
