---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: circulatepack.com
  spf: true
hosts:
- cert_expires: Dec 11 23:59:59 2026 GMT
  host: circulatepack.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Circulate Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Circulate, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Circulate
provider_slug: circulate
slug: circulate-domain-security
source_filename: circulate-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-08'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: circulatepack.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 11 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: circulatepack.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/circulate/refs/heads/main/security/circulate-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Packaging Data
- Compliance Reporting
- Sustainability
- ERP Integration
- API
- European Suppliers
- PPWR
---
