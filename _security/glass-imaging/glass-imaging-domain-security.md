---
description: ''
domains:
- caa:
  - cdn.webflow.com.
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: glass-imaging.com
  spf: false
hosts:
- cert_expires: Sep 21 20:27:55 2026 GMT
  host: www.glass-imaging.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Glass Imaging Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Glass Imaging, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF absent, DMARC present (p=none).'
provider_name: Glass Imaging
provider_slug: glass-imaging
slug: glass-imaging-domain-security
source_filename: glass-imaging-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.glass-imaging.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 21 20:27:55 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: glass-imaging.com\n  dnssec: true\n  caa:\n  - cdn.webflow.com.\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/glass-imaging/refs/heads/main/security/glass-imaging-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Ai
- Computational Photography
- Imaging
- Machine Learning
- Neural ISP
- Cameras
- Smartphones
---
