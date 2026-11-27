---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: devopness.com
  spf: false
hosts:
- cert_expires: Apr 14 23:59:59 2027 GMT
  host: devopness.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Devopness Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Devopness, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Devopness
provider_slug: devopness-com
slug: devopness-com-domain-security
source_filename: devopness-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: devopness.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Apr 14 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: devopness.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/devopness-com/security/devopness-com-domain-security.yml
summary_line: TLSv1.3
tags:
- Cloud
- Platform-as-a-Service
- DevOps
- Self-Hosted
- Infrastructure
---
