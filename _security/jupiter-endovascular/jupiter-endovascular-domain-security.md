---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: jupiterendo.com
  spf: true
hosts:
- cert_expires: Nov  1 13:08:28 2026 GMT
  host: jupiterendo.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Jupiter Endovascular Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Jupiter Endovascular, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Jupiter Endovascular
provider_slug: jupiter-endovascular
slug: jupiter-endovascular-domain-security
source_filename: jupiter-endovascular-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-23'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: jupiterendo.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  1 13:08:28 2026 GMT\n  hsts: false\ndomains:\n- domain: jupiterendo.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/jupiter-endovascular/refs/heads/main/security/jupiter-endovascular-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Medical Devices
- Medical Technology
- Healthcare
- Interventional Cardiology
- Pulmonary Embolism
- Clinical Trials
---
