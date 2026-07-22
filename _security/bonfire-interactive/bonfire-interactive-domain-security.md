---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: gobonfire.com
  spf: true
hosts:
- cert_expires: Oct 16 08:09:35 2026 GMT
  host: gobonfire.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Bonfire Interactive Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Bonfire Interactive, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Bonfire Interactive
provider_slug: bonfire-interactive
slug: bonfire-interactive-domain-security
source_filename: bonfire-interactive-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: gobonfire.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 16 08:09:35 2026 GMT\n  hsts: false\ndomains:\n- domain: gobonfire.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bonfire-interactive/refs/heads/main/security/bonfire-interactive-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Procurement
- Strategic Sourcing
- Public Sector
- GovTech
- Government
- Contract Management
- Supplier Management
- RFP
- SaaS
---
