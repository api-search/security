---
description: ''
domains:
- caa:
  - ;; connection timed out; no servers could be reached
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: opengamma.com
  spf: true
hosts:
- cert_expires: Sep  7 21:03:55 2026 GMT
  host: www.opengamma.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Opengamma Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for OpenGamma, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: OpenGamma
provider_slug: opengamma
slug: opengamma-domain-security
source_filename: opengamma-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.opengamma.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  7 21:03:55 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: opengamma.com\n  dnssec: false\n  caa:\n  - ;; connection timed out; no servers could be reached\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/opengamma/refs/heads/main/security/opengamma-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Fintech
- Derivatives
- Risk Management
- Analytics
- Margin
- Collateral
- Open Source
- Java
---
