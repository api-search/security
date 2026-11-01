---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: pku.edu.cn
  spf: true
hosts:
- cert_expires: Mar 24 05:59:59 2027 GMT
  host: iicsh.pku.edu.cn
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Iicsh Pku Edu Cn Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Peking University International Sci-Tech Innovation Center at Lin-gang Special Area, China (Shanghai) Pilot Free Trade Zone (PKU-IICSH), probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Peking University International Sci-Tech Innovation Center at Lin-gang Special Area, China (Shanghai) Pilot Free Trade Zone (PKU-IICSH)
provider_slug: iicsh-pku-edu-cn
slug: iicsh-pku-edu-cn-domain-security
source_filename: iicsh-pku-edu-cn-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: iicsh.pku.edu.cn\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 24 05:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: pku.edu.cn\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/iicsh-pku-edu-cn/security/iicsh-pku-edu-cn-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Innovation
- Research
- Technology
- Incubator
- China
- University
---
