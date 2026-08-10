---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: conceivable.life
  spf: true
hosts:
- cert_expires: Oct 24 14:24:53 2026 GMT
  host: www.conceivable.life
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Conceivable Life Sciences Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Conceivable Life Sciences, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Conceivable Life Sciences
provider_slug: conceivable-life-sciences
slug: conceivable-life-sciences-domain-security
source_filename: conceivable-life-sciences-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-09'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.conceivable.life\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 24 14:24:53 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: conceivable.life\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/conceivable-life-sciences/refs/heads/main/security/conceivable-life-sciences-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Health
- Fertility
- IVF
- Medical Devices
- Robotics
- Artificial Intelligence
- Life Sciences
- Laboratory Automation
---
