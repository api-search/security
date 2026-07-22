---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dmarc_rua: dmarc-reports@amusedco.com
  dnssec: false
  domain: amusedco.com
  nameservers:
  - stella.ns.cloudflare.com
  - quinton.ns.cloudflare.com
  spf: true
  spf_record: v=spf1 ip4:66.96.128.0/18 include:_spf.google.com ~all
hosts:
- behind: cloudflare
  host: amusedco.com
  hsts: true
  hsts_max_age: 7889238
  https: true
kind: domain-security
layout: security
method: probed
name: Thamarah Al Jill Co Llc Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Thamarah Al-Jill Co LLC, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS; 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Thamarah Al-Jill Co LLC
provider_slug: thamarah-al-jill-co-llc
slug: thamarah-al-jill-co-llc-domain-security
source_filename: thamarah-al-jill-co-llc-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: dig + TLS/HTTP HEAD against amusedco.com\nnotes: >-\n  amusedco.com is served through Cloudflare (Shopify store). HSTS is present on\n  agent/discovery paths (max-age observed 7889238). The storefront root returns a\n  Cloudflare managed-challenge 403 to non-browser clients. Absence of CAA / DNSSEC\n  records is recorded as observed, not inferred.\nhosts:\n  - host: amusedco.com\n    https: true\n    behind: cloudflare\n    hsts: true\n    hsts_max_age: 7889238\ndomains:\n  - domain: amusedco.com\n    nameservers: [stella.ns.cloudflare.com, quinton.ns.cloudflare.com]\n    dnssec: false\n    caa: []\n    spf: true\n    spf_record: 'v=spf1 ip4:66.96.128.0/18 include:_spf.google.com ~all'\n    dmarc: true\n    dmarc_policy: none\n    dmarc_rua: dmarc-reports@amusedco.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/thamarah-al-jill-co-llc/refs/heads/main/security/thamarah-al-jill-co-llc-domain-security.yml
summary_line: HSTS · DMARC
tags:
- Company
- E-commerce
- Marketplace
- Luxury
- Resale
- Fashion
- Agent Commerce
- Shopify
- Saudi Arabia
---
