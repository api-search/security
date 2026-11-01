---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: onedev.io
  spf: true
hosts:
- cert_expires: Jan  3 10:19:21 2027 GMT
  host: onedev.io
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Onedev Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for OneDev, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: OneDev
provider_slug: onedev
slug: onedev-domain-security
source_filename: onedev-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: onedev.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  3 10:19:21 2027 GMT\n  hsts: false\ndomains:\n- domain: onedev.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/onedev/security/onedev-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Development
- CI/CD
- Git
- Automation
---
