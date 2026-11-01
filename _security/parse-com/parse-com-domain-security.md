---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: parse.com
  spf: true
hosts:
- cert_expires: Oct 29 23:59:59 2026 GMT
  host: parse.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Parse Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Parse *, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Parse *
provider_slug: parse-com
slug: parse-com-domain-security
source_filename: parse-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-22'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: parse.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 29 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: parse.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/parse-com/security/parse-com-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
---
