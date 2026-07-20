---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: iqiyi.com
  spf: true
hosts:
- cert_expires: Jan 29 05:16:34 2027 GMT
  host: iqiyi.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Iqiyi Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for iQIYI, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: iQIYI
provider_slug: iqiyi
slug: iqiyi-domain-security
source_filename: iqiyi-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: iqiyi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 29 05:16:34 2027 GMT\n  hsts: false\ndomains:\n- domain: iqiyi.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/iqiyi/refs/heads/main/security/iqiyi-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Technology
- Video
- Streaming
- Media
- Entertainment
- OTT
- SaaS
---
