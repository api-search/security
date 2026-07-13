---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: blueprism.com
  spf: true
hosts:
- cert_expires: Sep  5 07:44:08 2026 GMT
  host: www.blueprism.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Blue Prism Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Blue Prism, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Blue Prism
provider_slug: blue-prism
slug: blue-prism-domain-security
source_filename: blue-prism-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.blueprism.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  5 07:44:08 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: blueprism.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/blue-prism/refs/heads/main/security/blue-prism-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- AI Automation
- RPA
---
