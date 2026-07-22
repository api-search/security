---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: ssi.inc
  spf: true
hosts:
- cert_expires: Sep 28 05:01:34 2026 GMT
  host: ssi.inc
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Safe Superintelligence Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Safe Superintelligence, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Safe Superintelligence
provider_slug: safe-superintelligence
slug: safe-superintelligence-domain-security
source_filename: safe-superintelligence-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ssi.inc\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 28 05:01:34 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: ssi.inc\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/safe-superintelligence/refs/heads/main/security/safe-superintelligence-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Artificial Intelligence
- Machine Learning
- AI Safety
- Research
- Superintelligence
---
