---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: koboldmetals.com
  spf: true
hosts:
- cert_expires: Sep 29 21:59:10 2026 GMT
  host: koboldmetals.com
  hsts: true
  hsts_max_age: 300
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Kobold Metals Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for KoBold Metals, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: KoBold Metals
provider_slug: kobold-metals
slug: kobold-metals-domain-security
source_filename: kobold-metals-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: koboldmetals.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 21:59:10 2026 GMT\n  hsts: true\n  hsts_max_age: 300\ndomains:\n- domain: koboldmetals.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kobold-metals/refs/heads/main/security/kobold-metals-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- American Dynamism
- Critical Minerals
- Mining
- Mineral Exploration
- Artificial Intelligence
- Machine Learning
- Geoscience
- Energy Transition
- Copper
---
