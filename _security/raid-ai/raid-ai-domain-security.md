---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: raidxai.com
  spf: true
hosts:
- cert_expires: Aug 27 13:01:14 2026 GMT
  host: raidxai.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  6 17:13:40 2026 GMT
  host: docs.raidxai.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 18 15:03:25 2026 GMT
  host: api.raidxai.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Raid Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Raid AI, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Raid AI
provider_slug: raid-ai
slug: raid-ai-domain-security
source_filename: raid-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: raidxai.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 27 13:01:14 2026 GMT\n  hsts: false\n- host: docs.raidxai.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  6 17:13:40 2026 GMT\n  hsts: false\n- host: api.raidxai.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 18 15:03:25 2026 GMT\n  hsts: null\ndomains:\n- domain: raidxai.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/raid-ai/refs/heads/main/security/raid-ai-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Deepfake Detection
- AI Content Detection
- Media Forensics
- Voice / Audio Detection
- Image Forensics
- Document Forensics
- Fact-Checking
- Trust & Safety
- Security
---
