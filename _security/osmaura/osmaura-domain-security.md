---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: osmaura.com
  spf: true
hosts:
- cert_expires: Sep 28 16:32:40 2026 GMT
  host: osmaura.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Osmaura Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Osmaura, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Osmaura
provider_slug: osmaura
slug: osmaura-domain-security
source_filename: osmaura-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: osmaura.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 28 16:32:40 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: osmaura.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/osmaura/refs/heads/main/security/osmaura-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Legal
- LegalTech
- Artificial Intelligence
- Sales Enablement
- Business Development
- Y Combinator
---
