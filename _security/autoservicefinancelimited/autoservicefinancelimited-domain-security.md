---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: bumper.co
  spf: true
hosts:
- cert_expires: Mar 25 23:59:59 2027 GMT
  host: www.bumper.co
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Autoservicefinancelimited Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Autoservicefinancelimited, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Autoservicefinancelimited
provider_slug: autoservicefinancelimited
slug: autoservicefinancelimited-domain-security
source_filename: autoservicefinancelimited-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.bumper.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 25 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: bumper.co\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/autoservicefinancelimited/refs/heads/main/security/autoservicefinancelimited-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Finance
- Automotive
- Fintech
- United Kingdom
- Payments
---
