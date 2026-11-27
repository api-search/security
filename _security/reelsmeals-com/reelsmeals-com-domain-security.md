---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dns_aid:
    checked: '2026-11-22'
    published: false
  dnssec: true
  domain: reelsmeals.com
  spf: true
hosts:
- cert_expires: Feb 14 10:57:55 2027 GMT
  host: reelsmeals.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: ReelsMeals Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ReelsMeals, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: ReelsMeals
provider_slug: reelsmeals-com
slug: reelsmeals-com-domain-security
source_filename: reelsmeals-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-22'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: reelsmeals.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 14 10:57:55 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: reelsmeals.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n  dns_aid:\n    checked: '2026-11-22'\n    published: false\n"
source_yaml_url: https://artifacts.apis.io/reelsmeals-com/security/reelsmeals-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Recipes
- Cooking
- Social-Media
- Meal-Planning
- Tools
---
