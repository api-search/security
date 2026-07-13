---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: mit.edu
  spf: true
hosts:
- cert_expires: Nov  7 23:59:59 2026 GMT
  host: web.mit.edu
  hsts: true
  hsts_max_age: 600
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Kerberos Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Kerberos, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Kerberos
provider_slug: kerberos
slug: kerberos-domain-security
source_filename: kerberos-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: web.mit.edu\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Nov  7 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 600\ndomains:\n- domain: mit.edu\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kerberos/refs/heads/main/security/kerberos-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Authentication
- Kerberos
- Security
- Single Sign-On
---
