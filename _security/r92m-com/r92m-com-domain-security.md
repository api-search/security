---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: r92m.com
  spf: true
hosts:
- cert_expires: Dec 14 14:29:42 2026 GMT
  host: r92m.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: R92M Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for R92m, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: R92m
provider_slug: r92m-com
slug: r92m-com-domain-security
source_filename: r92m-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: r92m.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 14 14:29:42 2026 GMT\n  hsts: false\ndomains:\n- domain: r92m.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/r92m-com/security/r92m-com-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Healthcare
- Technology
- Platform
- Medical
---
