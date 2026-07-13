---
api_specs:
- filename: proxmox-openapi.yml
  format: yaml
  label: Proxmox VE API
  slug: ve-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/proxmox/refs/heads/main/openapi/proxmox-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: proxmox.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: your.server
  spf: false
hosts:
- cert_expires: Sep 21 23:17:39 2026 GMT
  host: www.proxmox.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 23 21:19:44 2026 GMT
  host: pve.proxmox.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- host: your.server
  https: false
kind: domain-security
layout: security
method: probed
name: Proxmox Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Proxmox VE, probed live across 3 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Proxmox VE
provider_slug: proxmox
slug: proxmox-domain-security
source_filename: proxmox-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.proxmox.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 21 23:17:39 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: pve.proxmox.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 23 21:19:44 2026 GMT\n  hsts: false\n- host: your.server\n  https: false\ndomains:\n- domain: proxmox.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n- domain: your.server\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/proxmox/refs/heads/main/security/proxmox-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Virtualization
- KVM
- Containers
- LXC
- Clustering
- Open Source
---
