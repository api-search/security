---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: l3harris.com
  spf: true
hosts:
- cert_expires: Aug  7 21:53:15 2026 GMT
  host: www.l3harris.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: L3Harris Technologies Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for L3Harris Technologies, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: L3Harris Technologies
provider_slug: l3harris-technologies
slug: l3harris-technologies-domain-security
source_filename: l3harris-technologies-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.l3harris.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Aug  7 21:53:15 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: l3harris.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/l3harris-technologies/refs/heads/main/security/l3harris-technologies-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Aerospace
- Defense
- Fortune 500
- Government
---
