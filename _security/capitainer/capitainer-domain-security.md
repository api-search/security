---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: capitainer.com
  spf: true
hosts:
- cert_expires: Dec 28 03:05:37 2026 GMT
  host: capitainer.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Capitainer Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Capitainer, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Capitainer
provider_slug: capitainer
slug: capitainer-domain-security
source_filename: capitainer-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-07'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: capitainer.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 28 03:05:37 2026 GMT\n  hsts: false\ndomains:\n- domain: capitainer.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/capitainer/refs/heads/main/security/capitainer-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Microsampling
- Biotechnology
- Laboratory
- Instruments
---
