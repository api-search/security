---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: conkaymedical.com
  spf: false
hosts:
- cert_expires: Nov 14 07:16:41 2026 GMT
  host: www.conkaymedical.com
  hsts: true
  hsts_max_age: 0
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Conkay Medical Systems Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ConKay Medical Systems, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: ConKay Medical Systems
provider_slug: conkay-medical-systems
slug: conkay-medical-systems-domain-security
source_filename: conkay-medical-systems-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-10'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.conkaymedical.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 14 07:16:41 2026 GMT\n  hsts: true\n  hsts_max_age: 0\ndomains:\n- domain: conkaymedical.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/conkay-medical-systems/refs/heads/main/security/conkay-medical-systems-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Medical Devices
- Cardiovascular
- Valvular Regurgitation
- Early Stage
- Pleasanton
---
