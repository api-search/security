---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: truemeds.in
  spf: true
hosts:
- cert_expires: Oct 23 23:59:59 2026 GMT
  host: www.truemeds.in
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Truemeds Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Truemeds, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Truemeds
provider_slug: truemeds
slug: truemeds-domain-security
source_filename: truemeds-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.truemeds.in\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 23 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: truemeds.in\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/truemeds/refs/heads/main/security/truemeds-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Consumer
- Healthcare
- Pharmacy
- Medicine
- E-commerce
- Telehealth
- India
---
