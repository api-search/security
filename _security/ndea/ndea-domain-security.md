---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: ndea.com
  spf: true
hosts:
- cert_expires: Aug 30 03:52:50 2026 GMT
  host: ndea.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Ndea Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Ndea, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Ndea
provider_slug: ndea
slug: ndea-domain-security
source_filename: ndea-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ndea.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 30 03:52:50 2026 GMT\n  hsts: false\ndomains:\n- domain: ndea.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ndea/refs/heads/main/security/ndea-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Artificial Intelligence
- AGI
- Machine Learning
- Program Synthesis
- Deep Learning
- Reasoning
- Research Lab
- Science
---
