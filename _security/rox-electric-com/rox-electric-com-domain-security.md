---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: rox-electric.com
  spf: false
hosts:
- cert_expires: Dec  2 23:12:49 2026 GMT
  host: www.rox-electric.com
  hsts: null
  https: true
  tls_version: TLSv1.2
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Rox Electric Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Rox, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Rox
provider_slug: rox-electric-com
slug: rox-electric-com-domain-security
source_filename: rox-electric-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-22'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.rox-electric.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec  2 23:12:49 2026 GMT\n  hsts: null\ndomains:\n- domain: rox-electric.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/rox-electric-com/security/rox-electric-com-domain-security.yml
summary_line: TLSv1.2
tags:
- Company
---
