---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: edufund.in
  spf: true
hosts:
- cert_expires: Jan 14 04:59:51 2027 GMT
  host: www.edufund.in
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Edufund Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Edufund, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Edufund
provider_slug: edufund
slug: edufund-domain-security
source_filename: edufund-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-24'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.edufund.in\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 14 04:59:51 2027 GMT\n  hsts: false\ndomains:\n- domain: edufund.in\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/edufund/security/edufund-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Fintech
- Education
- Investment
- India
---
