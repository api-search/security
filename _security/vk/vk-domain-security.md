---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: vk.com
  spf: true
hosts:
- cert_expires: Jan  1 09:34:17 2027 GMT
  host: vk.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Vk Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for vk, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: vk
provider_slug: vk
slug: vk-domain-security
source_filename: vk-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: vk.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  1 09:34:17 2027 GMT\n  hsts: null\ndomains:\n- domain: vk.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vk/refs/heads/main/security/vk-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Social
- Public APIs
---
