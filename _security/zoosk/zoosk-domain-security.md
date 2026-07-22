---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: zoosk.com
  spf: true
hosts:
- cert_expires: Aug 15 10:51:47 2026 GMT
  host: www.zoosk.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Zoosk Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Zoosk, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Zoosk
provider_slug: zoosk
slug: zoosk-domain-security
source_filename: zoosk-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.zoosk.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 15 10:51:47 2026 GMT\n  hsts: false\ndomains:\n- domain: zoosk.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zoosk/refs/heads/main/security/zoosk-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Consumer
---
