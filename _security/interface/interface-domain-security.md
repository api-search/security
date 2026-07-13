---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: interface.com
  spf: true
hosts:
- cert_expires: Sep 11 19:36:01 2026 GMT
  host: www.interface.com
  hsts: true
  hsts_max_age: 5184000
  https: true
  tls_version: TLSv1.3
- host: developer.interface.com
  https: false
- host: api.interface.com
  https: false
kind: domain-security
layout: security
method: probed
name: Interface Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Interface Inc, probed live across 3 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Interface Inc
provider_slug: interface
slug: interface-domain-security
source_filename: interface-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.interface.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 11 19:36:01 2026 GMT\n  hsts: true\n  hsts_max_age: 5184000\n- host: developer.interface.com\n  https: false\n- host: api.interface.com\n  https: false\ndomains:\n- domain: interface.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/interface/refs/heads/main/security/interface-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Flooring
- Sustainability
- Commercial
---
