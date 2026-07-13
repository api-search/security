---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: gretel.ai
  spf: true
hosts:
- cert_expires: Nov 19 23:59:59 2026 GMT
  host: gretel.ai
  hsts: false
  https: true
  tls_version: TLSv1.2
- host: api.docs.gretel.ai
  https: false
- host: api.gretel.ai
  https: false
kind: domain-security
layout: security
method: probed
name: Gretel Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Gretel, probed live across 3 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Gretel
provider_slug: gretel-ai
slug: gretel-ai-domain-security
source_filename: gretel-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: gretel.ai\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Nov 19 23:59:59 2026 GMT\n  hsts: false\n- host: api.docs.gretel.ai\n  https: false\n- host: api.gretel.ai\n  https: false\ndomains:\n- domain: gretel.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gretel-ai/refs/heads/main/security/gretel-ai-domain-security.yml
summary_line: TLSv1.2 · DMARC
tags:
- Synthetic Data
- Privacy Engineering
- Tabular
- Text
- Time-Series
- REST
- Python SDK
- AI Data
---
