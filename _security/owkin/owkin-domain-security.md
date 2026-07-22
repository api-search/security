---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: owkin.com
  spf: true
hosts:
- cert_expires: Sep 17 18:58:41 2026 GMT
  host: owkin.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Owkin Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for OWKIN, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: OWKIN
provider_slug: owkin
slug: owkin-domain-security
source_filename: owkin-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: owkin.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 17 18:58:41 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: owkin.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/owkin/refs/heads/main/security/owkin-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- AI
- Biotech
- Drug Discovery
- Healthcare
- Machine Learning
- Precision Medicine
- Life Sciences
- Federated Learning
- Agentic AI
---
