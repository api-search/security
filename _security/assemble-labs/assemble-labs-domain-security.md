---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: assemblelabs.ai
  spf: true
hosts:
- cert_expires: Sep  3 09:58:43 2026 GMT
  host: assemblelabs.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Assemble Labs Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Assemble Labs, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Assemble Labs
provider_slug: assemble-labs
slug: assemble-labs-domain-security
source_filename: assemble-labs-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: assemblelabs.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  3 09:58:43 2026 GMT\n  hsts: false\ndomains:\n- domain: assemblelabs.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/assemble-labs/refs/heads/main/security/assemble-labs-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Hardware Testing
- Embedded Systems
- Firmware
- Test Automation
- Lab Automation
- Artificial Intelligence
---
