---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dns_aid:
    checked: '2026-11-25'
    published: false
  dnssec: false
  domain: syfert.com
  spf: true
hosts:
- cert_expires: Jan 16 15:19:33 2027 GMT
  host: syfert.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Syfert Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Syfert, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Syfert
provider_slug: syfert-com
slug: syfert-com-domain-security
source_filename: syfert-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-25'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: syfert.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 16 15:19:33 2027 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: syfert.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n  dns_aid:\n    checked: '2026-11-25'\n    published: false\n"
source_yaml_url: https://artifacts.apis.io/syfert-com/security/syfert-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- LegalTech
- AI
- Research
- Free
- OpenSource
---
