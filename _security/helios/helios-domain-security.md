---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: helios.do
  spf: true
hosts:
- cert_expires: Oct 25 02:27:59 2026 GMT
  host: www.helios.do
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Helios Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for helios, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: helios
provider_slug: helios
slug: helios-domain-security
source_filename: helios-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.helios.do\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 25 02:27:59 2026 GMT\n  hsts: false\ndomains:\n- domain: helios.do\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/helios/refs/heads/main/security/helios-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Banking
- Fintech
- Neobank
- Sustainable Finance
- Payments
- Climate Tech
- France
---
