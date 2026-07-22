---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: vibebio.com
  spf: true
hosts:
- cert_expires: Oct  2 11:29:05 2026 GMT
  host: vibebio.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Vibe Bio Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Vibe Bio, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Vibe Bio
provider_slug: vibe-bio
slug: vibe-bio-domain-security
source_filename: vibe-bio-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: vibebio.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 11:29:05 2026 GMT\n  hsts: false\ndomains:\n- domain: vibebio.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vibe-bio/refs/heads/main/security/vibe-bio-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
- Biopharma
- Artificial Intelligence
- Drug Discovery
- Business Development
- Life Sciences
- Rare Disease
- Venture Fund
---
