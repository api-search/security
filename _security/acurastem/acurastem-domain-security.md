---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: acurastem.com
  spf: true
hosts:
- cert_expires: Dec  1 13:35:38 2026 GMT
  host: acurastem.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Acurastem Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AcuraStem, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: AcuraStem
provider_slug: acurastem
slug: acurastem-domain-security
source_filename: acurastem-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-06'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: acurastem.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  1 13:35:38 2026 GMT\n  hsts: false\ndomains:\n- domain: acurastem.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/acurastem/refs/heads/main/security/acurastem-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Biotechnology
- Therapeutics
- Life Sciences
- Drug Discovery
- Neuroscience
- Neurodegenerative Disease
- ALS
- Stem Cells
- Machine Learning
- Private Company
---
