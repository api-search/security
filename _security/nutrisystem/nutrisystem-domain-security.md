---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: nutrisystem.com
  spf: true
hosts:
- cert_expires: Nov 25 23:59:59 2026 GMT
  host: www.nutrisystem.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Nutrisystem Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Nutrisystem (Wellina by Nutrisystem), probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Nutrisystem (Wellina by Nutrisystem)
provider_slug: nutrisystem
slug: nutrisystem-domain-security
source_filename: nutrisystem-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.nutrisystem.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 25 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: nutrisystem.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nutrisystem/refs/heads/main/security/nutrisystem-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Consumer Subscription
- Diet
- Direct To Consumer
- E Commerce
- Health And Wellness
- Meal Delivery
- Mobile App
- Nutrition
- Subscription Commerce
- Weight Loss
---
