---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: linkdrip.com
  spf: false
hosts:
- cert_expires: Jan 22 13:10:22 2027 GMT
  host: linkdrip.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Linkdrip Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for LinkDrip, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: LinkDrip
provider_slug: linkdrip
slug: linkdrip-domain-security
source_filename: linkdrip-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: linkdrip.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 22 13:10:22 2027 GMT\n  hsts: false\ndomains:\n- domain: linkdrip.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/linkdrip/security/linkdrip-domain-security.yml
summary_line: TLSv1.3
tags:
- Link Management
- No-Code
- Marketing
- Analytics
- URL Shortener
---
