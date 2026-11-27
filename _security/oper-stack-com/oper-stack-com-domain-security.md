---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: oper-stack.com
  spf: true
hosts:
- cert_expires: Dec 18 19:34:58 2026 GMT
  host: oper-stack.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: OperStack Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for OperStack, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: OperStack
provider_slug: oper-stack-com
slug: oper-stack-com-domain-security
source_filename: oper-stack-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: oper-stack.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 18 19:34:58 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: oper-stack.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/oper-stack-com/security/oper-stack-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Artificial Intelligence
- SEO
- Visibility
- Analytics
- Solo
---
