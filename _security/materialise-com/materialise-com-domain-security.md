---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: materialise.com
  spf: true
hosts:
- cert_expires: Jan 13 15:02:59 2027 GMT
  host: www.materialise.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Materialise Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Identify3D, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Identify3D
provider_slug: materialise-com
slug: materialise-com-domain-security
source_filename: materialise-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-24'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.materialise.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 13 15:02:59 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: materialise.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/materialise-com/security/materialise-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- 3DPrinting
- DigitalManufacturing
- AssetControl
- MedicalDevices
---
