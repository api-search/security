---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: humanlongevity.com
  spf: true
hosts:
- cert_expires: Nov 13 23:59:59 2026 GMT
  host: www.humanlongevity.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 27 12:23:09 2026 GMT
  host: auth.humanlongevity.com
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 31536000
  https: true
  note: Auth0 custom-domain authorization server for the HLI client portal; serves a real OpenID Connect discovery document.
  tls_version: TLSv1.3
- cert_expires: Oct  2 02:51:16 2026 GMT
  host: portal.humanlongevity.com
  hsts: false
  https: true
  note: HLI client portal (Angular SPA). No Strict-Transport-Security response header observed on the root document.
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Human Longevity Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Human Longevity, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Human Longevity
provider_slug: human-longevity
slug: human-longevity-domain-security
source_filename: human-longevity-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-22'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml hosts plus auth./portal. subdomains discovered in the client-portal\n  bundle\nhosts:\n- host: www.humanlongevity.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 13 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: auth.humanlongevity.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 27 12:23:09 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n  hsts_include_subdomains: true\n  note: Auth0 custom-domain authorization server for the HLI client portal; serves a real OpenID Connect\n    discovery document.\n- host: portal.humanlongevity.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 02:51:16 2026 GMT\n  hsts: false\n  note: HLI client portal (Angular SPA). No Strict-Transport-Security response header observed on the\n    root document.\ndomains:\n- domain: humanlongevity.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc:\
  \ true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/human-longevity/refs/heads/main/security/human-longevity-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Health
- Healthcare
- Genomics
- Precision Medicine
- Diagnostics
- Artificial Intelligence
- Longevity
- Life Sciences
- Medical Imaging
---
