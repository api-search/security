---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: ikigai.net
  spf: true
hosts:
- cert_expires: Oct  4 14:57:20 2026 GMT
  host: ikigai.net
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Ikigai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Ikigai, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Ikigai
provider_slug: ikigai
slug: ikigai-domain-security
source_filename: ikigai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ikigai.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 14:57:20 2026 GMT\n  hsts: false\ndomains:\n- domain: ikigai.net\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ikigai/refs/heads/main/security/ikigai-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
---
