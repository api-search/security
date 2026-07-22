---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: frontagelab.com.cn
  spf: true
hosts:
- cert_expires: Sep 15 20:36:30 2026 GMT
  host: frontagelab.com.cn
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Frontagelab Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Frontage Laboratories, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Frontage Laboratories
provider_slug: frontagelab
slug: frontagelab-domain-security
source_filename: frontagelab-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: frontagelab.com.cn\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 20:36:30 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: frontagelab.com.cn\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/frontagelab/refs/heads/main/security/frontagelab-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Contract Research Organization
- Pharmaceutical
- Biotechnology
- Drug Discovery
- Drug Development
- Bioanalysis
- Laboratory Testing
- CMC
- Life Sciences
---
