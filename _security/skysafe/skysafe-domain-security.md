---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: skysafe.io
  spf: true
hosts:
- cert_expires: Oct 10 23:59:59 2026 GMT
  host: www.skysafe.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Skysafe Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for SkySafe, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: SkySafe
provider_slug: skysafe
slug: skysafe-domain-security
source_filename: skysafe-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.skysafe.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 10 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: skysafe.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/skysafe/refs/heads/main/security/skysafe-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Drone Detection
- Counter-UAS
- Airspace Intelligence
- Security
- Public Safety
- Remote ID
- Signals Intelligence
---
