---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: propertypartner.co
  spf: true
hosts:
- cert_expires: Nov 12 23:59:59 2026 GMT
  host: propertypartner.co
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Propertypartner Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for London House Exchange (Property Partner), probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: London House Exchange (Property Partner)
provider_slug: propertypartner
slug: propertypartner-domain-security
source_filename: propertypartner-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: propertypartner.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 12 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: propertypartner.co\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/propertypartner/refs/heads/main/security/propertypartner-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Real Estate
- Property
- FinTech
- Investment
- Fractional Ownership
- PropTech
- United Kingdom
---
