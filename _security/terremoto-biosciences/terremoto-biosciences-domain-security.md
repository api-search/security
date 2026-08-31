---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: terremotobio.com
  spf: true
hosts:
- cert_expires: Nov 10 07:49:55 2026 GMT
  host: terremotobio.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Terremoto Biosciences Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Terremoto Biosciences, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Terremoto Biosciences
provider_slug: terremoto-biosciences
slug: terremoto-biosciences-domain-security
source_filename: terremoto-biosciences-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-30'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: terremotobio.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 10 07:49:55 2026 GMT\n  hsts: false\ndomains:\n- domain: terremotobio.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/terremoto-biosciences/refs/heads/main/security/terremoto-biosciences-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Biotechnology
- Pharmaceuticals
- Drug Discovery
- Life Sciences
- Oncology
- Healthcare
- Clinical Stage
- Small Molecule
---
