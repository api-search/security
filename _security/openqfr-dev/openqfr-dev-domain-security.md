---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: openqfr.dev
  spf: false
hosts:
- cert_expires: Feb  3 04:32:19 2027 GMT
  host: openqfr.dev
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: openqfr-dev Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for openqfr-dev, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: openqfr-dev
provider_slug: openqfr-dev
slug: openqfr-dev-domain-security
source_filename: openqfr-dev-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: openqfr.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  3 04:32:19 2027 GMT\n  hsts: null\ndomains:\n- domain: openqfr.dev\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/openqfr-dev/security/openqfr-dev-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
---
