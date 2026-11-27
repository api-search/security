---
description: ''
domains:
- caa: []
  dmarc: false
  dns_aid:
    checked: '2026-11-26'
    published: false
  dnssec: false
  domain: tessryx.io
  spf: false
hosts:
- cert_expires: Feb 18 23:48:18 2027 GMT
  host: tessryx.io
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Tessryx Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Tessryx, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Tessryx
provider_slug: tessryx-io
slug: tessryx-io-domain-security
source_filename: tessryx-io-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: tessryx.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 18 23:48:18 2027 GMT\n  hsts: false\ndomains:\n- domain: tessryx.io\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n  dns_aid:\n    checked: '2026-11-26'\n    published: false\n"
source_yaml_url: https://artifacts.apis.io/tessryx-io/security/tessryx-io-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
---
