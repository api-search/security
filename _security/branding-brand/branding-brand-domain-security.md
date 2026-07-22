---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: brandingbrand.com
  spf: true
hosts:
- cert_expires: Sep 25 23:59:59 2026 GMT
  host: www.brandingbrand.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Branding Brand Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Branding Brand, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Branding Brand
provider_slug: branding-brand
slug: branding-brand-domain-security
source_filename: branding-brand-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.brandingbrand.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 25 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: brandingbrand.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/branding-brand/refs/heads/main/security/branding-brand-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Commerce
- eCommerce
- Mobile
- React Native
- Retail
- Omnichannel
- Open Source
- SDK
- CLI
---
