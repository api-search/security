---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: accutarbio.com
  spf: true
hosts:
- cert_expires: Nov 30 10:56:34 2026 GMT
  host: www.accutarbio.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Accutar Biotechnology Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Accutar Biotechnology, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Accutar Biotechnology
provider_slug: accutar-biotechnology
slug: accutar-biotechnology-domain-security
source_filename: accutar-biotechnology-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-06'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.accutarbio.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 30 10:56:34 2026 GMT\n  hsts: false\ndomains:\n- domain: accutarbio.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/accutar-biotechnology/refs/heads/main/security/accutar-biotechnology-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Biotechnology
- Pharmaceuticals
- Drug Discovery
- Artificial Intelligence
- Machine Learning
- Cheminformatics
- Oncology
- Life Sciences
- Health
---
