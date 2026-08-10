---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: cagentvascular.com
  spf: true
hosts:
- cert_expires: Oct  5 04:29:51 2026 GMT
  host: cagentvascular.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Cagent Vascular Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cagent Vascular, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Cagent Vascular
provider_slug: cagent-vascular
slug: cagent-vascular-domain-security
source_filename: cagent-vascular-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-08'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: cagentvascular.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  5 04:29:51 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: cagentvascular.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cagent-vascular/refs/heads/main/security/cagent-vascular-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Medical Devices
- Healthcare
- Vascular
- Peripheral Artery Disease
- Endovascular
- Angioplasty
- MedTech
---
