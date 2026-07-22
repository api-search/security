---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: irhythmtech.com
  spf: true
hosts:
- cert_expires: Aug 30 15:53:12 2026 GMT
  host: irhythmtech.com
  hsts: true
  hsts_max_age: 31557600
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Irhythmtech Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Irhythmtech, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Irhythmtech
provider_slug: irhythmtech
slug: irhythmtech-domain-security
source_filename: irhythmtech-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: irhythmtech.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 30 15:53:12 2026 GMT\n  hsts: true\n  hsts_max_age: 31557600\ndomains:\n- domain: irhythmtech.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/irhythmtech/refs/heads/main/security/irhythmtech-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Healthcare
- Digital Health
- Cardiac Monitoring
- Medical Devices
- Remote Patient Monitoring
- Diagnostics
- Wearables
- Artificial Intelligence
---
