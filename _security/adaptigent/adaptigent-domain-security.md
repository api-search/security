---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: adaptigent.com
  spf: false
hosts:
- cert_expires: Aug 19 09:11:35 2026 GMT
  host: www.adaptigent.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Adaptigent Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Adaptigent, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF absent, DMARC present (p=reject).'
provider_name: Adaptigent
provider_slug: adaptigent
slug: adaptigent-domain-security
source_filename: adaptigent-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.adaptigent.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 19 09:11:35 2026 GMT\n  hsts: false\ndomains:\n- domain: adaptigent.com\n  dnssec: true\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/adaptigent/refs/heads/main/security/adaptigent-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Mainframe
- Integration
- API Gateway
- Legacy Systems
- Enterprise
- No Code
- Middleware
---
