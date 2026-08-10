---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: presidiomedical.com
  spf: true
hosts:
- cert_expires: Oct 26 12:03:00 2026 GMT
  host: presidiomedical.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Presidio Medical Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Presidio Medical, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Presidio Medical
provider_slug: presidio-medical
slug: presidio-medical-domain-security
source_filename: presidio-medical-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: presidiomedical.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 26 12:03:00 2026 GMT\n  hsts: null\ndomains:\n- domain: presidiomedical.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/presidio-medical/refs/heads/main/security/presidio-medical-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Medical Devices
- Neuromodulation
- Neurotechnology
- Spinal Cord Stimulation
- Chronic Pain
- Implantable Devices
- Clinical Stage
- Healthcare
- Life Sciences
---
