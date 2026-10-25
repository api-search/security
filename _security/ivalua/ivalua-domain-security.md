---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: ivalua.com
  spf: true
hosts:
- cert_expires: Jan 10 20:52:00 2027 GMT
  host: www.ivalua.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Ivalua Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Ivalua, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Ivalua
provider_slug: ivalua
slug: ivalua-domain-security
source_filename: ivalua-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.ivalua.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 10 20:52:00 2027 GMT\n  hsts: false\ndomains:\n- domain: ivalua.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ivalua/refs/heads/main/security/ivalua-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Procurement
- Source-to-Pay
- Supplier Management
- Contract Management
- Sourcing
- Purchase Orders
- Invoices
- Spend Analytics
- ERP Integration
- Enterprise
---
