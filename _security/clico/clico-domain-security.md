---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: cli.com
  spf: true
hosts:
- cert_expires: Dec 21 13:06:10 2026 GMT
  host: cli.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Clico Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Clico, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Clico
provider_slug: clico
slug: clico-domain-security
source_filename: clico-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: cli.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 21 13:06:10 2026 GMT\n  hsts: false\ndomains:\n- domain: cli.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/clico/refs/heads/main/security/clico-domain-security.yml
summary_line: TLSv1.3
tags:
- URL Shorteners
- Public APIs
---
