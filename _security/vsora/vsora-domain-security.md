---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: vsora.com
  spf: true
hosts:
- cert_expires: Oct 12 00:20:17 2026 GMT
  host: www.vsora.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Vsora Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for VSORA, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: VSORA
provider_slug: vsora
slug: vsora-domain-security
source_filename: vsora-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.vsora.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 12 00:20:17 2026 GMT\n  hsts: false\ndomains:\n- domain: vsora.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vsora/refs/heads/main/security/vsora-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Ai/Ml
- Semiconductors
- AI Inference
- Edge AI
- Hardware
- Data Centers
---
