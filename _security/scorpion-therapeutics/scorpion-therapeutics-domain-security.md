---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: scorpiontx.com
  spf: true
hosts:
- cert_expires: Dec  1 19:47:16 2026 GMT
  host: www.scorpiontx.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Scorpion Therapeutics Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Scorpion Therapeutics, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Scorpion Therapeutics
provider_slug: scorpion-therapeutics
slug: scorpion-therapeutics-domain-security
source_filename: scorpion-therapeutics-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.scorpiontx.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  1 19:47:16 2026 GMT\n  hsts: null\ndomains:\n- domain: scorpiontx.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/scorpion-therapeutics/refs/heads/main/security/scorpion-therapeutics-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Biotechnology
- Pharmaceuticals
- Oncology
- Precision Medicine
- Drug Discovery
- Life Sciences
- Clinical Research
---
