---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: briibio.com
  spf: true
hosts:
- cert_expires: Mar 27 23:59:59 2027 GMT
  host: www.briibio.com
  hsts: true
  hsts_max_age: 16070400
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Brii Biosciences Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Brii BioSciences, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Brii BioSciences
provider_slug: brii-biosciences
slug: brii-biosciences-domain-security
source_filename: brii-biosciences-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-06'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.briibio.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 27 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 16070400\ndomains:\n- domain: briibio.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/brii-biosciences/refs/heads/main/security/brii-biosciences-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Biotech
- Monoclonal Antibodies
- Infectious Diseases
- Hepatitis B
- COVID-19
- Neuroscience
- China
---
