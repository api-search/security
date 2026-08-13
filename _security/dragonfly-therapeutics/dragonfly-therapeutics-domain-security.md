---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: dragonflytx.com
  spf: true
hosts:
- cert_expires: Sep 29 02:19:34 2026 GMT
  host: www.dragonflytx.com
  hsts: true
  hsts_max_age: 31556952
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Dragonfly Therapeutics Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Dragonfly Therapeutics, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Dragonfly Therapeutics
provider_slug: dragonfly-therapeutics
slug: dragonfly-therapeutics-domain-security
source_filename: dragonfly-therapeutics-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.dragonflytx.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 02:19:34 2026 GMT\n  hsts: true\n  hsts_max_age: 31556952\ndomains:\n- domain: dragonflytx.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dragonfly-therapeutics/refs/heads/main/security/dragonfly-therapeutics-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Biotechnology
- Pharmaceuticals
- Immunotherapy
- Oncology
- Life Sciences
- Clinical Stage
- Drug Discovery
- Healthcare
---
