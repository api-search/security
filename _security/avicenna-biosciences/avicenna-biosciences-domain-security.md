---
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 issue "sectigo.com"
  dmarc: false
  dnssec: false
  domain: avicenna-bio.com
  spf: true
hosts:
- cert_expires: Sep 20 05:21:49 2026 GMT
  host: www.avicenna-bio.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Avicenna Biosciences Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Avicenna Biosciences, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Avicenna Biosciences
provider_slug: avicenna-biosciences
slug: avicenna-biosciences-domain-security
source_filename: avicenna-biosciences-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.avicenna-bio.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 20 05:21:49 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: avicenna-bio.com\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"sectigo.com\"\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/avicenna-biosciences/refs/heads/main/security/avicenna-biosciences-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Biosciences
- Life Sciences
- Biotechnology
- Venture Backed
- DCVC Portfolio
- Drug Discovery
- Machine Learning
- Medicinal Chemistry
- Small Molecule
- Neurodegenerative Disease
- Artificial Intelligence
---
