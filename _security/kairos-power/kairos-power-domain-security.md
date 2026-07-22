---
description: ''
domains:
- caa:
  - 0 issue "pki.goog"
  - 0 issue "amazonaws.com"
  - 0 issuewild "amazonaws.com"
  - 0 issue "amazon.com"
  - 0 issuewild "amazon.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: kairospower.com
  spf: true
hosts:
- cert_expires: Aug 17 16:32:57 2026 GMT
  host: kairospower.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Kairos Power Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Kairos Power, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Kairos Power
provider_slug: kairos-power
slug: kairos-power-domain-security
source_filename: kairos-power-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: kairospower.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 17 16:32:57 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: kairospower.com\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  - 0 issue \"amazonaws.com\"\n  - 0 issuewild \"amazonaws.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issuewild \"amazon.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kairos-power/refs/heads/main/security/kairos-power-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Nuclear
- Advanced Nuclear
- Nuclear Fission
- Small Modular Reactor
- Generation IV
- KP-FHR
- Fluoride Salt
- TRISO Fuel
- Hermes Reactor
- Energy
- Clean Energy
- Power Generation
- Hyperscaler Power
---
