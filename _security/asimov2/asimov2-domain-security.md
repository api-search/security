---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: asimov.com
  spf: true
hosts:
- cert_expires: Nov 10 00:41:44 2026 GMT
  host: www.asimov.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Asimov2 Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Asimov2, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Asimov2
provider_slug: asimov2
slug: asimov2-domain-security
source_filename: asimov2-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.asimov.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 10 00:41:44 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: asimov.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/asimov2/refs/heads/main/security/asimov2-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Placeholder
- Harvest
- Stub
- API-Evangelist
---
