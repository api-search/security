---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: causalens.com
  spf: true
hosts:
- cert_expires: Oct  9 01:47:27 2026 GMT
  host: causalens.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  6 07:30:07 2026 GMT
  host: dara.causalens.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Causalens Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for CausaLens, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: CausaLens
provider_slug: causalens
slug: causalens-domain-security
source_filename: causalens-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-09'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: causalens.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  9 01:47:27 2026 GMT\n  hsts: false\n- host: dara.causalens.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  6 07:30:07 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: causalens.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/causalens/refs/heads/main/security/causalens-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Artificial Intelligence
- Causal AI
- Machine-Learning
- Data Science
- Decision Intelligence
- Analytics
- Agents
- Open-Source
- Python
---
