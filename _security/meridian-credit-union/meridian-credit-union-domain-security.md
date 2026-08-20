---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: meridiancu.ca
  spf: true
hosts:
- cert_expires: Sep 23 10:29:08 2026 GMT
  host: www.meridiancu.ca
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Meridian Credit Union Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Meridian Credit Union, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Meridian Credit Union
provider_slug: meridian-credit-union
slug: meridian-credit-union-domain-security
source_filename: meridian-credit-union-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-23'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.meridiancu.ca\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 23 10:29:08 2026 GMT\n  hsts: false\ndomains:\n- domain: meridiancu.ca\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/meridian-credit-union/refs/heads/main/security/meridian-credit-union-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Financial-Services
- Banking
- Canada
- Credit Union
- Cooperative
- Ontario
- Data Aggregation
---
