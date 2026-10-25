---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: sigmahealthcare.com.au
  spf: true
hosts:
- cert_expires: Nov 23 19:00:41 2026 GMT
  host: sigmahealthcare.com.au
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Sigma Healthcare Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Sigma Healthcare, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Sigma Healthcare
provider_slug: sigma-healthcare
slug: sigma-healthcare-domain-security
source_filename: sigma-healthcare-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-22'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: sigmahealthcare.com.au\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 23 19:00:41 2026 GMT\n  hsts: false\ndomains:\n- domain: sigmahealthcare.com.au\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sigma-healthcare/refs/heads/main/security/sigma-healthcare-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Healthcare
- Pharmacy
- Pharmaceutical Distribution
- Wholesale
- Logistics
- Retail
- Australia
---
