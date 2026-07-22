---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: kooapp.com
  spf: true
hosts:
- cert_expires: Aug 17 16:55:18 2026 GMT
  host: www.kooapp.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Koo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Koo, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Koo
provider_slug: koo
slug: koo-domain-security
source_filename: koo-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.kooapp.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 17 16:55:18 2026 GMT\n  hsts: null\ndomains:\n- domain: kooapp.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/koo/refs/heads/main/security/koo-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Social
- Social Networking
- Microblogging
- India
- Consumer
- Defunct
---
