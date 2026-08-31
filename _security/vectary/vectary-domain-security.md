---
description: ''
domains:
- caa:
  - 0 iodef "mailto:security@vectary.com"
  - 128 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: vectary.com
  spf: true
hosts:
- cert_expires: Oct  3 11:12:55 2026 GMT
  host: www.vectary.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Vectary Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Vectary, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Vectary
provider_slug: vectary
slug: vectary-domain-security
source_filename: vectary-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.vectary.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 11:12:55 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: vectary.com\n  dnssec: false\n  caa:\n  - 0 iodef \"mailto:security@vectary.com\"\n  - 128 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vectary/refs/heads/main/security/vectary-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Design Tech
- 3D Design
- Augmented Reality
- 3D Configurator
- Product Visualization
- ECommerce
---
