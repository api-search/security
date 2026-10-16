---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: corsha.com
  spf: true
hosts:
- cert_expires: Nov 26 03:48:03 2026 GMT
  host: corsha.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Corsha Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Corsha, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Corsha
provider_slug: corsha
slug: corsha-domain-security
source_filename: corsha-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: corsha.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 26 03:48:03 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: corsha.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/corsha/refs/heads/main/security/corsha-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Security
- Industrial
- Identity
- OT
---
