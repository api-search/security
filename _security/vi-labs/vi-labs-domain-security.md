---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: vi.co
  spf: true
hosts:
- cert_expires: Nov 12 14:27:56 2026 GMT
  host: vi.co
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Vi Labs Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Vi Labs, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Vi Labs
provider_slug: vi-labs
slug: vi-labs-domain-security
source_filename: vi-labs-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: vi.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 12 14:27:56 2026 GMT\n  hsts: false\ndomains:\n- domain: vi.co\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vi-labs/refs/heads/main/security/vi-labs-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Artificial Intelligence
- Health
- Healthcare
- Life Sciences
- Pharmaceuticals
- Patient Engagement
- Enterprise AI
- AI Agents
- Model Context Protocol
- Data
---
