---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: scottsmiraclegro.com
  spf: true
hosts:
- cert_expires: Dec 10 23:59:59 2026 GMT
  host: scottsmiraclegro.com
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Scotts Miracle Gro Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for The Scotts Miracle-Gro Company, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: The Scotts Miracle-Gro Company
provider_slug: scotts-miracle-gro
slug: scotts-miracle-gro-domain-security
source_filename: scotts-miracle-gro-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: scottsmiraclegro.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec 10 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: scottsmiraclegro.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/scotts-miracle-gro/refs/heads/main/security/scotts-miracle-gro-domain-security.yml
summary_line: TLSv1.2 · DMARC
tags:
- consumer-products
- lawn-and-garden
- manufacturing
- retail
- ecommerce
- agriculture
- home-and-garden
---
