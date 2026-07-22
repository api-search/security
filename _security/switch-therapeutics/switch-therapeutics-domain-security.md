---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: switchthera.com
  spf: true
hosts:
- cert_expires: Aug 28 20:03:21 2026 GMT
  host: www.switchthera.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Switch Therapeutics Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Switch Therapeutics, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Switch Therapeutics
provider_slug: switch-therapeutics
slug: switch-therapeutics-domain-security
source_filename: switch-therapeutics-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.switchthera.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 28 20:03:21 2026 GMT\n  hsts: false\ndomains:\n- domain: switchthera.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/switch-therapeutics/refs/heads/main/security/switch-therapeutics-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
- Biotech
- Biotechnology
- Pharmaceuticals
- Genetic Medicine
- RNAi
- Neuroscience
- Life Sciences
---
