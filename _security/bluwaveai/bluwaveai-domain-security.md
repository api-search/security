---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: bluwave-ai.com
  spf: true
hosts:
- cert_expires: Nov  6 03:20:23 2026 GMT
  host: www.bluwave-ai.com
  hsts: true
  hsts_max_age: 31557600
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Bluwaveai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Bluwaveai, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Bluwaveai
provider_slug: bluwaveai
slug: bluwaveai-domain-security
source_filename: bluwaveai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-29'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.bluwave-ai.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  6 03:20:23 2026 GMT\n  hsts: true\n  hsts_max_age: 31557600\ndomains:\n- domain: bluwave-ai.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bluwaveai/refs/heads/main/security/bluwaveai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Artificial Intelligence
- Clean Energy
- Smart Grid
- Energy Storage
- Data Center
- Electric Vehicles
- Utilities
---
