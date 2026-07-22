---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: theblandcompany.co
  spf: true
hosts:
- cert_expires: Oct  1 01:15:19 2026 GMT
  host: www.theblandcompany.co
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Bland Company Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Bland Company, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Bland Company
provider_slug: bland-company
slug: bland-company-domain-security
source_filename: bland-company-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.theblandcompany.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 01:15:19 2026 GMT\n  hsts: false\ndomains:\n- domain: theblandcompany.co\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bland-company/refs/heads/main/security/bland-company-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Frontier Tech
- Food Tech
- Biotechnology
- Plant Protein
- Egg Replacement
- Ingredients
- Sustainability
---
