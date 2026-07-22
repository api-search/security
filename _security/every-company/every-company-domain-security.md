---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: theeverycompany.com
  spf: true
hosts:
- cert_expires: Aug 29 23:29:41 2026 GMT
  host: theeverycompany.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Every Company Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for EVERY Company, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: EVERY Company
provider_slug: every-company
slug: every-company-domain-security
source_filename: every-company-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: theeverycompany.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 29 23:29:41 2026 GMT\n  hsts: false\ndomains:\n- domain: theeverycompany.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/every-company/refs/heads/main/security/every-company-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Foodtech
- Precision Fermentation
- Alternative Protein
- Food Ingredients
- Animal-Free
- Sustainability
---
