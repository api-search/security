---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: getfuchsia.ai
  spf: true
hosts:
- cert_expires: Aug 30 20:31:31 2026 GMT
  host: getfuchsia.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Fuchsia Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Fuchsia, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Fuchsia
provider_slug: fuchsia
slug: fuchsia-domain-security
source_filename: fuchsia-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: getfuchsia.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 30 20:31:31 2026 GMT\n  hsts: false\ndomains:\n- domain: getfuchsia.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fuchsia/refs/heads/main/security/fuchsia-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Hardware
- Certification
- Compliance
- Regulatory
- Testing
- Hardware Compliance
- AI Agents
- Robotics
- Medical Devices
- IoT
---
