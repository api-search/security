---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: defaultrank.com
  spf: true
hosts:
- cert_expires: Dec 30 08:26:52 2026 GMT
  host: defaultrank.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: DefaultRank Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for DefaultRank, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: DefaultRank
provider_slug: defaultrank-com
slug: defaultrank-com-domain-security
source_filename: defaultrank-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: defaultrank.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 30 08:26:52 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: defaultrank.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/defaultrank-com/security/defaultrank-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Artificial Intelligence
- Developer Tools
- Rankings
- Analytics
---
