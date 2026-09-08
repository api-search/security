---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: expeditors.com
  spf: true
hosts:
- cert_expires: Mar  3 23:59:59 2027 GMT
  host: www.expeditors.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 15 23:59:59 2026 GMT
  host: help.expeditors.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 20 23:59:59 2026 GMT
  host: api.expeditors.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Expeditors International Of Washington Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Expeditors International of Washington, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Expeditors International of Washington
provider_slug: expeditors-international-of-washington
slug: expeditors-international-of-washington-domain-security
source_filename: expeditors-international-of-washington-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-07'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.expeditors.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar  3 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: help.expeditors.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 23:59:59 2026 GMT\n  hsts: null\n- host: api.expeditors.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 20 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: expeditors.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/expeditors-international-of-washington/refs/heads/main/security/expeditors-international-of-washington-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Customs
- Freight Forwarding
- Logistics
- Supply Chain
- Warehousing
- Shipment Tracking
- Transportation
- Order Management
- Customs Brokerage
- Visibility
---
