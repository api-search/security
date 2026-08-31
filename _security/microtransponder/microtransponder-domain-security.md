---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: mobia.com
  spf: true
hosts:
- cert_expires: Oct 30 19:01:48 2026 GMT
  host: www.mobia.com
  hsts: true
  hsts_max_age: 300
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Microtransponder Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for MicroTransponder, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: MicroTransponder
provider_slug: microtransponder
slug: microtransponder-domain-security
source_filename: microtransponder-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-25'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.mobia.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 30 19:01:48 2026 GMT\n  hsts: true\n  hsts_max_age: 300\ndomains:\n- domain: mobia.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/microtransponder/refs/heads/main/security/microtransponder-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Medical Devices
- Healthcare
- Neurotechnology
- Neuromodulation
- Stroke Rehabilitation
- Implantable Devices
- Life Sciences
- WordPress
- MCP
---
