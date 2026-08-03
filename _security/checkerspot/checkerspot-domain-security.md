---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: checkerspot.com
  spf: true
hosts:
- cert_expires: Sep 18 04:03:03 2026 GMT
  host: www.checkerspot.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Checkerspot Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Checkerspot, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Checkerspot
provider_slug: checkerspot
slug: checkerspot-domain-security
source_filename: checkerspot-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.checkerspot.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 18 04:03:03 2026 GMT\n  hsts: false\ndomains:\n- domain: checkerspot.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/checkerspot/refs/heads/main/security/checkerspot-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Biotechnology
- Precision Fermentation
- Synthetic Biology
- Microalgae
- Lipids
- Fats and Oils
- Ingredients
- Infant Nutrition
- Food Technology
- Cosmetics
- Personal Care
- Materials
- Sustainability
- United States
---
