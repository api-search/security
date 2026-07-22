---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: ailylabs.com
  spf: true
hosts:
- cert_expires: Sep  4 14:07:48 2026 GMT
  host: ailylabs.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Aily Labs Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Aily Labs, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Aily Labs
provider_slug: aily-labs
slug: aily-labs-domain-security
source_filename: aily-labs-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ailylabs.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  4 14:07:48 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: ailylabs.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aily-labs/refs/heads/main/security/aily-labs-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Healthcare
- Life Sciences
- Artificial Intelligence
- Decision Intelligence
- Enterprise Software
- Predictive Analytics
- Supply Chain
- Munich
---
