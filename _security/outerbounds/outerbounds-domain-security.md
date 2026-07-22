---
description: ''
domains:
- caa:
  - cdn.webflow.com.
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: outerbounds.com
  spf: true
hosts:
- cert_expires: Sep  3 18:12:08 2026 GMT
  host: outerbounds.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Outerbounds Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Outerbounds, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Outerbounds
provider_slug: outerbounds
slug: outerbounds-domain-security
source_filename: outerbounds-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: outerbounds.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  3 18:12:08 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: outerbounds.com\n  dnssec: true\n  caa:\n  - cdn.webflow.com.\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/outerbounds/refs/heads/main/security/outerbounds-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Data Analytics
- Machine Learning
- MLOps
- Artificial Intelligence
- Data Science
- Metaflow
- Compute
- Python
---
