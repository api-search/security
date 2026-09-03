---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: vialase.com
  spf: true
hosts:
- cert_expires: Nov 11 09:44:27 2026 GMT
  host: www.vialase.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Vialase Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ViaLase, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: ViaLase
provider_slug: vialase
slug: vialase-domain-security
source_filename: vialase-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.vialase.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 11 09:44:27 2026 GMT\n  hsts: false\ndomains:\n- domain: vialase.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vialase/refs/heads/main/security/vialase-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Medical Devices
- Healthcare
- MedTech
- Ophthalmology
- Glaucoma
- Femtosecond Laser
- Surgical Devices
- Clinical Trials
- Medical Imaging
---
