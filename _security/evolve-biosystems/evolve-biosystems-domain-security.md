---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: infinanthealth.com
  spf: true
hosts:
- cert_expires: Sep 27 10:57:49 2026 GMT
  host: www.infinanthealth.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Evolve Biosystems Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Infinant Health, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Infinant Health
provider_slug: evolve-biosystems
slug: evolve-biosystems-domain-security
source_filename: evolve-biosystems-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.infinanthealth.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 27 10:57:49 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: infinanthealth.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/evolve-biosystems/refs/heads/main/security/evolve-biosystems-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Biotechnology
- Life Sciences
- Health
- Infant Nutrition
- Microbiome
- Probiotics
- Consumer Health
- Pharmaceuticals
- Clinical Research
---
