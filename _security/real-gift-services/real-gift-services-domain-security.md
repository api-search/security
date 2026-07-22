---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: getrealgifts.com
  spf: true
hosts:
- cert_expires: Aug 25 16:14:06 2026 GMT
  host: www.getrealgifts.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Real Gift Services Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Real Gift Services, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Real Gift Services
provider_slug: real-gift-services
slug: real-gift-services-domain-security
source_filename: real-gift-services-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.getrealgifts.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 25 16:14:06 2026 GMT\n  hsts: null\ndomains:\n- domain: getrealgifts.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/real-gift-services/refs/heads/main/security/real-gift-services-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
- Gifting
- Gift Cards
- Rewards
- Loyalty
- E-Commerce
- Commerce
- Embedded Commerce
- API
- SDKs
- Webhooks
---
