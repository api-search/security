---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: biointellisense.com
  spf: true
hosts:
- cert_expires: Oct 18 21:38:03 2026 GMT
  host: www.biointellisense.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 26 20:28:17 2026 GMT
  host: biocloud.biointellisense.com
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Biointellisense Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for BioIntelliSense, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: BioIntelliSense
provider_slug: biointellisense
slug: biointellisense-domain-security
source_filename: biointellisense-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.biointellisense.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 18 21:38:03 2026 GMT\n  hsts: false\n- host: biocloud.biointellisense.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec 26 20:28:17 2026 GMT\n  hsts: null\ndomains:\n- domain: biointellisense.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/biointellisense/refs/heads/main/security/biointellisense-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Health
- Healthcare
- Remote Patient Monitoring
- Wearables
- Medical Devices
- Vital Signs
- Continuous Monitoring
- Digital Health
- Data as a Service
---
