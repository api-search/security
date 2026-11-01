---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: moskitos.io
  spf: false
hosts:
- cert_expires: Nov 29 08:12:41 2026 GMT
  host: moskitos.io
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Moskitos Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for MOSKITOS, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: MOSKITOS
provider_slug: moskitos
slug: moskitos-domain-security
source_filename: moskitos-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: moskitos.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 29 08:12:41 2026 GMT\n  hsts: null\ndomains:\n- domain: moskitos.io\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/moskitos/security/moskitos-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
---
