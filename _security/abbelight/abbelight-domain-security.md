---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: abbelight.com
  spf: true
hosts:
- cert_expires: Oct 18 15:03:40 2026 GMT
  host: www.abbelight.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Abbelight Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Abbelight, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Abbelight
provider_slug: abbelight
slug: abbelight-domain-security
source_filename: abbelight-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.abbelight.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 18 15:03:40 2026 GMT\n  hsts: false\ndomains:\n- domain: abbelight.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/abbelight/refs/heads/main/security/abbelight-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
- Bioimaging
- Microscopy
- Nanoscopy
- Super Resolution
- Scientific Instruments
- Life Sciences
- Laboratory
- Medical Devices
- France
---
