---
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: nexaaly.com
  spf: true
hosts:
- cert_expires: Nov 23 17:19:38 2026 GMT
  host: nexaaly.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Nexaaly Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Nexaaly, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Nexaaly
provider_slug: nexaaly-com
slug: nexaaly-com-domain-security
source_filename: nexaaly-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: nexaaly.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 23 17:19:38 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: nexaaly.com\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/nexaaly-com/security/nexaaly-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Software
- Artificial Intelligence
- High Performance
- Denmark
- Research
---
