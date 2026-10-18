---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: carboncapture.com
  spf: true
hosts:
- cert_expires: Nov 17 23:04:04 2026 GMT
  host: www.carboncapture.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Carbon Capture Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Carbon Capture, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Carbon Capture
provider_slug: carbon-capture
slug: carbon-capture-domain-security
source_filename: carbon-capture-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-07'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.carboncapture.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 17 23:04:04 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: carboncapture.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/carbon-capture/refs/heads/main/security/carbon-capture-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- DirectAirCapture
- CarbonRemoval
- Climate Tech
- CleanEnergy
---
