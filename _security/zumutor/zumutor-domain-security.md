---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: zumutor.com
  spf: true
hosts:
- cert_expires: Sep 30 14:19:40 2026 GMT
  host: www.zumutor.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Zumutor Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Zumutor, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Zumutor
provider_slug: zumutor
slug: zumutor-domain-security
source_filename: zumutor-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.zumutor.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 14:19:40 2026 GMT\n  hsts: false\ndomains:\n- domain: zumutor.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zumutor/refs/heads/main/security/zumutor-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Healthcare
---
