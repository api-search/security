---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: uniandes.edu.co
  spf: true
hosts:
- cert_expires: Sep  9 05:44:19 2026 GMT
  host: www.uniandes.edu.co
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  9 01:43:17 2026 GMT
  host: repositorio.uniandes.edu.co
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: University Of Los Andes Colombia Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for University of Los Andes Colombia, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: University of Los Andes Colombia
provider_slug: university-of-los-andes-colombia
slug: university-of-los-andes-colombia-domain-security
source_filename: university-of-los-andes-colombia-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.uniandes.edu.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  9 05:44:19 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: repositorio.uniandes.edu.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  9 01:43:17 2026 GMT\n  hsts: null\ndomains:\n- domain: uniandes.edu.co\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/university-of-los-andes-colombia/refs/heads/main/security/university-of-los-andes-colombia-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Education
- Higher Education
- University
- Colombia
- Latin America
- Open Access
- Institutional Repository
- Research
---
