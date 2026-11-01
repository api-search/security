---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: hitachi.com
  spf: true
hosts:
- cert_expires: Apr 11 23:59:59 2027 GMT
  host: www.hitachi.com
  hsts: true
  hsts_max_age: 31557600
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Hitachi Ltd Central Research Laboratory Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Hitachi, Ltd., Central Research Laboratory, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Hitachi, Ltd., Central Research Laboratory
provider_slug: hitachi-ltd-central-research-laboratory
slug: hitachi-ltd-central-research-laboratory-domain-security
source_filename: hitachi-ltd-central-research-laboratory-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.hitachi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Apr 11 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31557600\ndomains:\n- domain: hitachi.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/hitachi-ltd-central-research-laboratory/security/hitachi-ltd-central-research-laboratory-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Research
- Technology
- Innovation
- Hitachi
---
