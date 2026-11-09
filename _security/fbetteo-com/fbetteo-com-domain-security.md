---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: fbetteo.com
  spf: false
hosts:
- cert_expires: Dec 10 16:40:20 2026 GMT
  host: fbetteo.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Fbetteo Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for fbetteo-com, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: fbetteo-com
provider_slug: fbetteo-com
slug: fbetteo-com-domain-security
source_filename: fbetteo-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-07'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: fbetteo.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 10 16:40:20 2026 GMT\n  hsts: false\ndomains:\n- domain: fbetteo.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/fbetteo-com/security/fbetteo-com-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
---
