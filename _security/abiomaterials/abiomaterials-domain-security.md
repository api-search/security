---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: a-bio.co.kr
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: a-biousa.com
  spf: true
hosts:
- cert_expires: Feb  1 23:59:59 2027 GMT
  host: a-bio.co.kr
  hsts: false
  https: true
  tls_version: TLSv1.2
- cert_expires: Dec  3 15:41:57 2026 GMT
  host: a-biousa.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 2
kind: domain-security
layout: security
method: probed
name: Abiomaterials Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for A-Bio Materials, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: A-Bio Materials
provider_slug: abiomaterials
slug: abiomaterials-domain-security
source_filename: abiomaterials-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-06'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: a-bio.co.kr\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Feb  1 23:59:59 2027 GMT\n  hsts: false\n- host: a-biousa.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  3 15:41:57 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: a-bio.co.kr\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n- domain: a-biousa.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/abiomaterials/refs/heads/main/security/abiomaterials-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Company
- Biomaterials
- Life Sciences
- Cosmetics
- Medical Devices
- Exosomes
- Manufacturing
- E-Commerce
- South Korea
---
