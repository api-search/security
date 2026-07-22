---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: endovascularengineering.com
  spf: true
hosts:
- cert_expires: Sep  8 23:13:01 2026 GMT
  host: endovascularengineering.com
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Endovascularengineering Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Endovascularengineering, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Endovascularengineering
provider_slug: endovascularengineering
slug: endovascularengineering-domain-security
source_filename: endovascularengineering-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: endovascularengineering.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep  8 23:13:01 2026 GMT\n  hsts: false\ndomains:\n- domain: endovascularengineering.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/endovascularengineering/refs/heads/main/security/endovascularengineering-domain-security.yml
summary_line: TLSv1.2 · DMARC
tags:
- Company
- Medical Devices
- Endovascular
- Thrombectomy
- Cardiovascular
- Pulmonary Embolism
- Health
- Interventional
---
