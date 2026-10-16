---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: japanpost.jp
  spf: true
hosts:
- cert_expires: Mar  8 04:49:49 2027 GMT
  host: www.post.japanpost.jp
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Japan Post Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Japan Post, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Japan Post
provider_slug: japan-post
slug: japan-post-domain-security
source_filename: japan-post-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.post.japanpost.jp\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar  8 04:49:49 2027 GMT\n  hsts: false\ndomains:\n- domain: japanpost.jp\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/japan-post/refs/heads/main/security/japan-post-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Postal
- Logistics
- Finance
- E‑services
---
