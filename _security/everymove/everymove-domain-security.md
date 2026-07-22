---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: everymove.org
  spf: true
hosts:
- cert_expires: Dec  9 23:59:59 2026 GMT
  host: everymove.org
  hsts: true
  hsts_max_age: 2600000
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Everymove Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for EveryMove, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: EveryMove
provider_slug: everymove
slug: everymove-domain-security
source_filename: everymove-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: everymove.org\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec  9 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 2600000\ndomains:\n- domain: everymove.org\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/everymove/refs/heads/main/security/everymove-domain-security.yml
summary_line: TLSv1.2 · HSTS · DNSSEC · DMARC
tags:
- Company
---
