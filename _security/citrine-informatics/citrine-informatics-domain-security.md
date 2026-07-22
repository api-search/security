---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: citrine.io
  spf: true
hosts:
- cert_expires: Sep 27 04:49:17 2026 GMT
  host: citrine.io
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Citrine Informatics Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Citrine Informatics, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Citrine Informatics
provider_slug: citrine-informatics
slug: citrine-informatics-domain-security
source_filename: citrine-informatics-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: citrine.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 27 04:49:17 2026 GMT\n  hsts: false\ndomains:\n- domain: citrine.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/citrine-informatics/refs/heads/main/security/citrine-informatics-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Materials Informatics
- Artificial Intelligence
- Machine Learning
- Chemicals
- Materials Science
- Generative AI
- SDK
- Python
---
