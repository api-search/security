---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: vitalconnect.com
  spf: true
hosts:
- cert_expires: Oct 17 17:04:01 2026 GMT
  host: vitalconnect.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Vitalconnect Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for VitalConnect, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: VitalConnect
provider_slug: vitalconnect
slug: vitalconnect-domain-security
source_filename: vitalconnect-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: vitalconnect.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 17 17:04:01 2026 GMT\n  hsts: false\ndomains:\n- domain: vitalconnect.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vitalconnect/refs/heads/main/security/vitalconnect-domain-security.yml
summary_line: TLSv1.3
tags:
- Health
- Healthcare
- Medical Devices
- Remote Patient Monitoring
- Cardiac Monitoring
- Biosensors
- Wearables
- Telehealth
- Clinical Trials
- Webhooks
---
