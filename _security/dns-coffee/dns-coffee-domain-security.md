---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: dns.coffee
  spf: false
hosts:
- cert_expires: Sep  5 05:38:03 2026 GMT
  host: dns.coffee
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  5 05:38:03 2026 GMT
  host: api.dns.coffee
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Dns Coffee Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for DNS Coffee, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF absent, DMARC present (p=none).'
provider_name: DNS Coffee
provider_slug: dns-coffee
slug: dns-coffee-domain-security
source_filename: dns-coffee-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: dns.coffee\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  5 05:38:03 2026 GMT\n  hsts: false\n- host: api.dns.coffee\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  5 05:38:03 2026 GMT\n  hsts: false\ndomains:\n- domain: dns.coffee\n  dnssec: true\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dns-coffee/refs/heads/main/security/dns-coffee-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- DNS
- Domain Names
- Domains
---
