---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: doorstead.com
  spf: true
hosts:
- cert_expires: Sep 25 14:26:20 2026 GMT
  host: www.doorstead.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Doorstead Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Doorstead, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Doorstead
provider_slug: doorstead
slug: doorstead-domain-security
source_filename: doorstead-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.doorstead.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 25 14:26:20 2026 GMT\n  hsts: false\ndomains:\n- domain: doorstead.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/doorstead/refs/heads/main/security/doorstead-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
- Property Management
- Real-Estate
- PropTech
- Rental
- Leasing
- Residential
- Tenant Screening
---
