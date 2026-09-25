---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: perfectday.com
  spf: true
hosts:
- cert_expires: Sep 25 07:42:21 2026 GMT
  host: perfectday.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Perfect Day Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Perfect Day, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Perfect Day
provider_slug: perfect-day
slug: perfect-day-domain-security
source_filename: perfect-day-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: perfectday.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 25 07:42:21 2026 GMT\n  hsts: false\ndomains:\n- domain: perfectday.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/perfect-day/refs/heads/main/security/perfect-day-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Food Technology
- Precision Fermentation
- Alternative Protein
- Ingredients
- Sustainability
- Biotechnology
- Consumer Packaged Goods
- content-api
- WordPress
---
