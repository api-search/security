---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: virtualincision.com
  spf: true
hosts:
- cert_expires: Oct 27 18:13:27 2026 GMT
  host: virtualincision.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Virtual Incision Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Virtual Incision, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Virtual Incision
provider_slug: virtual-incision
slug: virtual-incision-domain-security
source_filename: virtual-incision-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: virtualincision.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 27 18:13:27 2026 GMT\n  hsts: false\ndomains:\n- domain: virtualincision.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/virtual-incision/refs/heads/main/security/virtual-incision-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Medical Devices
- Surgical Robotics
- Robotics
- Healthcare
- Health
- Life Sciences
- Medical Technology
- Content
- News
- Careers
- Event
- MCP
---
