---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: blameless.com
  spf: true
hosts:
- cert_expires: Sep  8 16:16:09 2026 GMT
  host: www.blameless.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Blameless Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Blameless, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Blameless
provider_slug: blameless
slug: blameless-domain-security
source_filename: blameless-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.blameless.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  8 16:16:09 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: blameless.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/blameless/refs/heads/main/security/blameless-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- AIOps
- SRE
---
