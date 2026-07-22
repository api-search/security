---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: invivyd.com
  spf: true
hosts:
- cert_expires: Aug 28 13:36:59 2026 GMT
  host: www.invivyd.com
  hsts: true
  hsts_max_age: 31622400
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Adagio Therapeutics Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Adagio Therapeutics, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Adagio Therapeutics
provider_slug: adagio-therapeutics
slug: adagio-therapeutics-domain-security
source_filename: adagio-therapeutics-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.invivyd.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 28 13:36:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31622400\ndomains:\n- domain: invivyd.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/adagio-therapeutics/refs/heads/main/security/adagio-therapeutics-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Life Sciences
- Biotechnology
- Pharmaceuticals
- Antibody Therapeutics
- Infectious Diseases
---
