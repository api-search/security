---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: pelagepharma.com
  spf: true
hosts:
- cert_expires: Sep 29 08:27:43 2026 GMT
  host: pelagepharma.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Pelage Pharmaceuticals Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Pelage Pharmaceuticals, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Pelage Pharmaceuticals
provider_slug: pelage-pharmaceuticals
slug: pelage-pharmaceuticals-domain-security
source_filename: pelage-pharmaceuticals-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: pelagepharma.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 08:27:43 2026 GMT\n  hsts: false\ndomains:\n- domain: pelagepharma.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pelage-pharmaceuticals/refs/heads/main/security/pelage-pharmaceuticals-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Life Sciences
- Pharmaceuticals
- Biotechnology
- Regenerative Medicine
- Clinical Trials
- Dermatology
---
