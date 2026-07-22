---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: policypal.com
  spf: false
hosts:
- cert_expires: Aug 24 08:40:56 2026 GMT
  host: policypal.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Policypal Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for PolicyPal, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: PolicyPal
provider_slug: policypal
slug: policypal-domain-security
source_filename: policypal-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: policypal.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 24 08:40:56 2026 GMT\n  hsts: false\ndomains:\n- domain: policypal.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/policypal/refs/heads/main/security/policypal-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- InsurTech
- FinTech
- Insurance
- Insurance Broker
- Personal Finance
- Singapore
---
