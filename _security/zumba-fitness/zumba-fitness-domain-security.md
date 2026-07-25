---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: zumba.com
  spf: true
hosts:
- cert_expires: Oct  4 21:10:34 2026 GMT
  host: www.zumba.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Zumba Fitness Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Zumba Fitness, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Zumba Fitness
provider_slug: zumba-fitness
slug: zumba-fitness-domain-security
source_filename: zumba-fitness-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.zumba.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 21:10:34 2026 GMT\n  hsts: null\ndomains:\n- domain: zumba.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zumba-fitness/refs/heads/main/security/zumba-fitness-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
---
