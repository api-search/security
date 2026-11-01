---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: js.design
  spf: true
hosts:
- cert_expires: Feb 17 23:59:59 2027 GMT
  host: js.design
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Instant Design Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Instant Design, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Instant Design
provider_slug: instant-design
slug: instant-design-domain-security
source_filename: instant-design-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-25'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: js.design\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 17 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: js.design\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/instant-design/security/instant-design-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
---
