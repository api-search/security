---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: ulta.com
  spf: true
hosts:
- cert_expires: Oct 16 23:59:59 2026 GMT
  host: www.ulta.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Ulta Salon Cosmetics And Fragrance Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Ulta Salon, Cosmetics & Fragrance, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Ulta Salon, Cosmetics & Fragrance
provider_slug: ulta-salon-cosmetics-and-fragrance
slug: ulta-salon-cosmetics-and-fragrance-domain-security
source_filename: ulta-salon-cosmetics-and-fragrance-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.ulta.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 16 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: ulta.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ulta-salon-cosmetics-and-fragrance/refs/heads/main/security/ulta-salon-cosmetics-and-fragrance-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Beauty
- Retail
- Cosmetics
- Fragrance
- Salon
---
