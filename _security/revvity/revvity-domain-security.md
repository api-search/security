---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: revvity.com
  spf: true
hosts:
- cert_expires: Sep 27 01:11:58 2026 GMT
  host: www.revvity.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Revvity Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Revvity, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Revvity
provider_slug: revvity
slug: revvity-domain-security
source_filename: revvity-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.revvity.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 27 01:11:58 2026 GMT\n  hsts: null\ndomains:\n- domain: revvity.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/revvity/refs/heads/main/security/revvity-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Life Sciences
- Diagnostics
- Healthcare
- Laboratory
- Biotechnology
---
