---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: hungrypanda.co
  spf: true
hosts:
- cert_expires: Nov 18 06:36:34 2026 GMT
  host: www.hungrypanda.co
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 24 18:35:38 2026 GMT
  host: api-uk-f2e.hungrypanda.co
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Hungrypanda Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for HungryPanda, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: HungryPanda
provider_slug: hungrypanda
slug: hungrypanda-domain-security
source_filename: hungrypanda-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-22'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.hungrypanda.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 18 06:36:34 2026 GMT\n  hsts: false\n- host: api-uk-f2e.hungrypanda.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 24 18:35:38 2026 GMT\n  hsts: false\ndomains:\n- domain: hungrypanda.co\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hungrypanda/refs/heads/main/security/hungrypanda-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
- Food Delivery
- Delivery
- Marketplace
- Restaurant
- Grocery
- Logistics
- E-Commerce
- Merchants
- Point-of-Sale
---
