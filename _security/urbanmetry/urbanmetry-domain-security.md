---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: urbanmetry.com
  spf: true
hosts:
- cert_expires: Oct 18 06:20:19 2026 GMT
  host: urbanmetry.com
  hsts: true
  hsts_max_age: 31556952
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Urbanmetry Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for UrbanMetry, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: UrbanMetry
provider_slug: urbanmetry
slug: urbanmetry-domain-security
source_filename: urbanmetry-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: urbanmetry.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct 18 06:20:19 2026 GMT\n  hsts: true\n  hsts_max_age: 31556952\ndomains:\n- domain: urbanmetry.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/urbanmetry/refs/heads/main/security/urbanmetry-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Company
- Real Estate
- Property
- Geospatial Analytics
- Urban Planning
- Data Analytics
- Location Intelligence
- Malaysia
---
