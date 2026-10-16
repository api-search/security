---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: coinone.co.kr
  spf: true
hosts:
- cert_expires: Dec 10 05:01:17 2026 GMT
  host: coinone.co.kr
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Coinone Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Coinone, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Coinone
provider_slug: coinone
slug: coinone-domain-security
source_filename: coinone-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-09'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: coinone.co.kr\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 10 05:01:17 2026 GMT\n  hsts: null\ndomains:\n- domain: coinone.co.kr\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/coinone/refs/heads/main/security/coinone-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
---
