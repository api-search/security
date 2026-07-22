---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: hq.xyz
  spf: true
hosts:
- cert_expires: Sep 16 14:27:15 2026 GMT
  host: hq.xyz
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Hq Headquarters Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for HQ, Headquarters, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: HQ, Headquarters
provider_slug: hq-headquarters
slug: hq-headquarters-domain-security
source_filename: hq-headquarters-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: hq.xyz\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 16 14:27:15 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: hq.xyz\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hq-headquarters/refs/heads/main/security/hq-headquarters-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
---
