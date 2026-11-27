---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dns_aid:
    checked: '2026-11-26'
    published: false
  dnssec: true
  domain: temsor.com
  spf: true
hosts:
- cert_expires: Jan 31 03:33:51 2027 GMT
  host: temsor.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Temsor Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Temsor, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Temsor
provider_slug: temsor-com
slug: temsor-com-domain-security
source_filename: temsor-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: temsor.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 31 03:33:51 2027 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: temsor.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n  dns_aid:\n    checked: '2026-11-26'\n    published: false\n"
source_yaml_url: https://artifacts.apis.io/temsor-com/security/temsor-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- AI
- Voice
- Communications
- SaaS
- Telephony
---
