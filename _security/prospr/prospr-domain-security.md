---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: prospr.work
  spf: true
hosts:
- cert_expires: Feb  3 23:59:59 2027 GMT
  host: prospr.work
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Prospr Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Prospr, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Prospr
provider_slug: prospr
slug: prospr-domain-security
source_filename: prospr-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: prospr.work\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  3 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: prospr.work\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/prospr/security/prospr-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- SaaS
- Frontline Management
- Collaboration
- Scheduling
---
