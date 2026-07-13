---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: realtyna.com
  spf: true
hosts:
- cert_expires: Oct  6 22:31:31 2026 GMT
  host: realtyna.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Realtyna Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Realtyna, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Realtyna
provider_slug: realtyna
slug: realtyna-domain-security
source_filename: realtyna-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: realtyna.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  6 22:31:31 2026 GMT\n  hsts: false\ndomains:\n- domain: realtyna.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/realtyna/refs/heads/main/security/realtyna-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Real Estate
- MLS
- IDX
- RESO
- WordPress
---
