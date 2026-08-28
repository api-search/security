---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: plantiblefoods.com
  spf: true
hosts:
- cert_expires: Oct 14 15:47:43 2026 GMT
  host: www.plantiblefoods.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Plantible Foods Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Plantible Foods, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Plantible Foods
provider_slug: plantible-foods
slug: plantible-foods-domain-security
source_filename: plantible-foods-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.plantiblefoods.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 14 15:47:43 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: plantiblefoods.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/plantible-foods/refs/heads/main/security/plantible-foods-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Food
- Food Ingredients
- Alternative Protein
- Plant-Based
- Agriculture
- Biotechnology
- Manufacturing
- Sustainability
- Texas
---
