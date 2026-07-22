---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: vipthink.net
  spf: false
hosts:
- cert_expires: Dec 11 23:59:59 2026 GMT
  host: vipthink.net
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Vipthink Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for VIPThink, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: VIPThink
provider_slug: vipthink
slug: vipthink-domain-security
source_filename: vipthink-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: vipthink.net\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec 11 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: vipthink.net\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vipthink/refs/heads/main/security/vipthink-domain-security.yml
summary_line: TLSv1.2
tags:
- Company
- Edtech
- Education
- Online Learning
- Mathematics
- Early Childhood Education
- China
- Consumer
---
