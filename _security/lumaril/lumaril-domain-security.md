---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: lumaril.com
  spf: true
hosts:
- cert_expires: Sep 28 20:30:23 2026 GMT
  host: lumaril.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Lumaril Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Lumaril, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Lumaril
provider_slug: lumaril
slug: lumaril-domain-security
source_filename: lumaril-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: lumaril.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 28 20:30:23 2026 GMT\n  hsts: false\ndomains:\n- domain: lumaril.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lumaril/refs/heads/main/security/lumaril-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Deep Tech
---
