---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: boostb2b.com
  spf: true
hosts:
- cert_expires: Dec  8 15:58:07 2026 GMT
  host: www.boostb2b.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Boost Payment Solutions Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Boost Payment Solutions, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Boost Payment Solutions
provider_slug: boost-payment-solutions
slug: boost-payment-solutions-domain-security
source_filename: boost-payment-solutions-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.boostb2b.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  8 15:58:07 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: boostb2b.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/boost-payment-solutions/refs/heads/main/security/boost-payment-solutions-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Payments
- FinTech
- B2B
- CommercialCards
- API
---
