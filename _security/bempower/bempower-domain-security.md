---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: bempower.org
  spf: true
hosts:
- cert_expires: Jan  5 23:59:59 2027 GMT
  host: bempower.org
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Bempower Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Bempower, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Bempower
provider_slug: bempower
slug: bempower-domain-security
source_filename: bempower-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-27'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: bempower.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  5 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: bempower.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bempower/refs/heads/main/security/bempower-domain-security.yml
summary_line: TLSv1.3
tags:
- Non-Profit
- Development
- Education
- Water
- Climate
---
