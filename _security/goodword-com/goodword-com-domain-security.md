---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: goodword.com
  spf: true
hosts:
- cert_expires: Feb  3 14:19:44 2027 GMT
  host: goodword.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Goodword Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Goodword, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Goodword
provider_slug: goodword-com
slug: goodword-com-domain-security
source_filename: goodword-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-10'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: goodword.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  3 14:19:44 2027 GMT\n  hsts: false\ndomains:\n- domain: goodword.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/goodword-com/security/goodword-com-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Artificial Intelligence
- Relationship Management
- Platform
- Founders
- Operator
---
