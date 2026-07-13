---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: avocode.com
  spf: true
hosts:
- cert_expires: Oct  1 12:14:38 2026 GMT
  host: avocode.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Avocode Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Avocode, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Avocode
provider_slug: avocode
slug: avocode-domain-security
source_filename: avocode-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: avocode.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 12:14:38 2026 GMT\n  hsts: false\ndomains:\n- domain: avocode.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/avocode/refs/heads/main/security/avocode-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Design
- Design Handoff
- Developer Collaboration
- Inspect
- Design Files
- Sketch
- Figma
- Adobe XD
- CSS Export
---
