---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: evidentvascular.com
  spf: true
hosts:
- cert_expires: Sep 22 15:05:06 2026 GMT
  host: evidentvascular.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Evident Vascular Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Evident Vascular, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Evident Vascular
provider_slug: evident-vascular
slug: evident-vascular-domain-security
source_filename: evident-vascular-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: evidentvascular.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 22 15:05:06 2026 GMT\n  hsts: false\ndomains:\n- domain: evidentvascular.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/evident-vascular/refs/heads/main/security/evident-vascular-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Medical Devices
- Health
- Imaging
- Artificial Intelligence
- Cardiovascular
- Ultrasound
- Medical Imaging
---
