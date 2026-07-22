---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: comfyapp.com
  spf: true
hosts:
- cert_expires: Oct  9 14:50:06 2026 GMT
  host: comfyapp.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Comfy Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Comfy *, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Comfy *
provider_slug: comfy
slug: comfy-domain-security
source_filename: comfy-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: comfyapp.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  9 14:50:06 2026 GMT\n  hsts: false\ndomains:\n- domain: comfyapp.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/comfy/refs/heads/main/security/comfy-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
- Frontier Tech
- Workplace Experience
- Smart Buildings
- PropTech
- Internet of Things
- Acquired
---
