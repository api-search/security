---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: labgeniustx.com
  spf: false
hosts:
- cert_expires: Sep  1 18:10:49 2026 GMT
  host: labgeniustx.com
  hsts: true
  hsts_max_age: 300
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Labgenius Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for LabGenius Therapeutics, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=quarantine).'
provider_name: LabGenius Therapeutics
provider_slug: labgenius
slug: labgenius-domain-security
source_filename: labgenius-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: labgeniustx.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  1 18:10:49 2026 GMT\n  hsts: true\n  hsts_max_age: 300\ndomains:\n- domain: labgeniustx.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/labgenius/refs/heads/main/security/labgenius-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Biotechnology
- Drug Discovery
- Therapeutics
- Antibodies
- Machine Learning
- Artificial Intelligence
- Life Sciences
- Oncology
- Laboratory Automation
- Synthetic Biology
---
