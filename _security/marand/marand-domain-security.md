---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: marand.com
  spf: true
hosts:
- cert_expires: Oct  8 09:01:41 2026 GMT
  host: www.marand.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Marand Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Marand, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Marand
provider_slug: marand
slug: marand-domain-security
source_filename: marand-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.marand.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  8 09:01:41 2026 GMT\n  hsts: false\ndomains:\n- domain: marand.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/marand/refs/heads/main/security/marand-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Telecommunications
- Business Support Systems
- BSS
- TM Forum
- Open Digital Architecture
- Open API
- Product Catalog
- CPQ
- CRM
- Billing
- Enterprise Software
- Standards Conformance
- Slovenia
---
