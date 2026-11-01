---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: whu.edu.cn
  spf: true
hosts:
- cert_expires: Mar 17 23:59:59 2027 GMT
  host: luojia.whu.edu.cn
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Hubei Luojia Laboratory Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Hubei Luojia Laboratory, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Hubei Luojia Laboratory
provider_slug: hubei-luojia-laboratory
slug: hubei-luojia-laboratory-domain-security
source_filename: hubei-luojia-laboratory-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: luojia.whu.edu.cn\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 17 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: whu.edu.cn\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/hubei-luojia-laboratory/security/hubei-luojia-laboratory-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Research
- Aerospace
- RemoteSensing
- Innovation
---
