---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: policygenius.com
  spf: true
hosts:
- cert_expires: Oct 21 18:02:43 2026 GMT
  host: policygenius.com
  hsts: true
  hsts_max_age: 900
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Policygenius Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Policygenius, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Policygenius
provider_slug: policygenius
slug: policygenius-domain-security
source_filename: policygenius-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: policygenius.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct 21 18:02:43 2026 GMT\n  hsts: true\n  hsts_max_age: 900\ndomains:\n- domain: policygenius.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/policygenius/refs/heads/main/security/policygenius-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Company
- Insurance
- InsurTech
- Life Insurance
- Marketplace
- Comparison
- Financial Services
- Consumer
---
