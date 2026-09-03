---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: vantisvascular.com
  spf: true
hosts:
- cert_expires: Oct 30 01:24:18 2026 GMT
  host: vantisvascular.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Vantis Vascular Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Vantis Vascular, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Vantis Vascular
provider_slug: vantis-vascular
slug: vantis-vascular-domain-security
source_filename: vantis-vascular-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: vantisvascular.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 30 01:24:18 2026 GMT\n  hsts: false\ndomains:\n- domain: vantisvascular.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vantis-vascular/refs/heads/main/security/vantis-vascular-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Medical Devices
- Health Care
- Cardiovascular
- Interventional Cardiology
- Vascular
- Catheters
- Medical Technology
---
