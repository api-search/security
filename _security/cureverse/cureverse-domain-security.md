---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: cureverse.co.kr
  spf: true
hosts:
- cert_expires: Jan  1 23:59:59 2027 GMT
  host: www.cureverse.co.kr
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Cureverse Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cureverse, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Cureverse
provider_slug: cureverse
slug: cureverse-domain-security
source_filename: cureverse-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.cureverse.co.kr\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  1 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: cureverse.co.kr\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cureverse/refs/heads/main/security/cureverse-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
---
