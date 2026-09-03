---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: utilityglobal.com
  spf: true
hosts:
- cert_expires: Oct 10 22:21:04 2026 GMT
  host: utilityglobal.com
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Utility Global Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Utility Global, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Utility Global
provider_slug: utility-global
slug: utility-global-domain-security
source_filename: utility-global-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: utilityglobal.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct 10 22:21:04 2026 GMT\n  hsts: false\ndomains:\n- domain: utilityglobal.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/utility-global/refs/heads/main/security/utility-global-domain-security.yml
summary_line: TLSv1.2 · DMARC
tags:
- Company
- Energy
- Hydrogen
- Decarbonization
- Clean Energy
- Industrial
- Steel
- Climate Tech
- Chemicals
---
