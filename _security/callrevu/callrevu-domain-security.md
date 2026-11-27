---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: callrevu.com
  spf: true
hosts:
- cert_expires: Feb  1 23:20:04 2027 GMT
  host: callrevu.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: CallRevu Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for CallRevu, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: CallRevu
provider_slug: callrevu
slug: callrevu-domain-security
source_filename: callrevu-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-16'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: callrevu.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  1 23:20:04 2027 GMT\n  hsts: null\ndomains:\n- domain: callrevu.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/callrevu/security/callrevu-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
---
