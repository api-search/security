---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: nexlab.net
  spf: true
hosts:
- cert_expires: Dec  9 03:46:11 2026 GMT
  host: nexlab.net
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Nexlab Net Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for nexlab-net, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: nexlab-net
provider_slug: nexlab-net
slug: nexlab-net-domain-security
source_filename: nexlab-net-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: nexlab.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  9 03:46:11 2026 GMT\n  hsts: false\ndomains:\n- domain: nexlab.net\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/nexlab-net/security/nexlab-net-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Technology
- Placeholder
- Unknown
- Stub
---
