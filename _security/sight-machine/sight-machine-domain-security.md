---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: sightmachine.com
  spf: true
hosts:
- cert_expires: Oct 31 21:37:16 2026 GMT
  host: www.sightmachine.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 23 19:23:48 2026 GMT
  host: docs.sightmachine.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Sight Machine Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Sight Machine, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Sight Machine
provider_slug: sight-machine
slug: sight-machine-domain-security
source_filename: sight-machine-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-27'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.sightmachine.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 31 21:37:16 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.sightmachine.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 23 19:23:48 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: sightmachine.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sight-machine/refs/heads/main/security/sight-machine-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Manufacturing
- Industrial IoT
- Analytics
- Artificial Intelligence
- Agents
- Data
- OPC UA
- MQTT
- Digital Twin
- Operations
---
