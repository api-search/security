---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: kubos.com
  spf: true
hosts:
- cert_expires: Dec  3 12:58:48 2026 GMT
  host: kubos.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Kubos Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Kubos, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Kubos
provider_slug: kubos
slug: kubos-domain-security
source_filename: kubos-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: kubos.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  3 12:58:48 2026 GMT\n  hsts: false\ndomains:\n- domain: kubos.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kubos/refs/heads/main/security/kubos-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Satellite
- Remote Sensing
- Data as a Service
- Edge Computing
- Ground Operations
- Hyperspectral Imaging
---
