---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: vexcel-imaging.com
  spf: true
hosts:
- cert_expires: Dec 25 18:04:15 2026 GMT
  host: www.vexcel-imaging.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Vexcel Imaging Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Vexcel Imaging, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Vexcel Imaging
provider_slug: vexcel-imaging
slug: vexcel-imaging-domain-security
source_filename: vexcel-imaging-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.vexcel-imaging.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 25 18:04:15 2026 GMT\n  hsts: false\ndomains:\n- domain: vexcel-imaging.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vexcel-imaging/refs/heads/main/security/vexcel-imaging-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Aerial Imaging
- Photogrammetry
- Mapping
- UltraCam
---
