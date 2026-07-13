---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: ttec.com
  spf: true
hosts:
- cert_expires: Oct  5 23:45:50 2026 GMT
  host: www.ttec.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- host: developer.ttec.com
  https: false
- host: api.ttec.com
  https: false
kind: domain-security
layout: security
method: probed
name: Teletech Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for TTEC Holdings, probed live across 3 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: TTEC Holdings
provider_slug: teletech
slug: teletech-domain-security
source_filename: teletech-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.ttec.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  5 23:45:50 2026 GMT\n  hsts: null\n- host: developer.ttec.com\n  https: false\n- host: api.ttec.com\n  https: false\ndomains:\n- domain: ttec.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/teletech/refs/heads/main/security/teletech-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Customer Experience
- Technology
- BPO
---
