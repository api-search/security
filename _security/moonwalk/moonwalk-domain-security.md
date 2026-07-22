---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: true
  domain: moonwalk.bio
  spf: true
hosts:
- cert_expires: Sep  3 10:53:38 2026 GMT
  host: moonwalk.bio
  hsts: true
  hsts_max_age: 300
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Moonwalk Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Moonwalk Biosciences, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC absent.'
provider_name: Moonwalk Biosciences
provider_slug: moonwalk
slug: moonwalk-domain-security
source_filename: moonwalk-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: moonwalk.bio\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  3 10:53:38 2026 GMT\n  hsts: true\n  hsts_max_age: 300\ndomains:\n- domain: moonwalk.bio\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/moonwalk/refs/heads/main/security/moonwalk-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC
tags:
- Company
- Biotechnology
- Therapeutics
- Epigenetics
- Obesity
- Healthcare
- Drug Discovery
- Life Sciences
---
