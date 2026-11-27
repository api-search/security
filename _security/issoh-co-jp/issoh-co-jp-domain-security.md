---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: issoh.co.jp
  spf: true
hosts:
- cert_expires: Jan 12 08:09:59 2027 GMT
  host: issoh.co.jp
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: ISSOH Co., Ltd. Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ISSOH Co., Ltd., probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: ISSOH Co., Ltd.
provider_slug: issoh-co-jp
slug: issoh-co-jp-domain-security
source_filename: issoh-co-jp-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: issoh.co.jp\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 12 08:09:59 2027 GMT\n  hsts: null\ndomains:\n- domain: issoh.co.jp\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/issoh-co-jp/security/issoh-co-jp-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- System Development
- Enterprise Software
- Cloud Services
- Japan
---
