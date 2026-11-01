---
description: ''
domains:
- caa:
  - 0 issuewild "amazontrust.com"
  - 0 issuewild "awstrust.com"
  - 0 issuewild "godaddy.com"
  - 0 issuewild "starfieldtech.com"
  - 0 iodef "mailto:admin@cronometer.com"
  - 0 issuewild "amazon.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: cronometer.com
  spf: true
hosts:
- cert_expires: Jan  7 23:59:59 2027 GMT
  host: cronometer.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Cronometer Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cronometer, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Cronometer
provider_slug: cronometer
slug: cronometer-domain-security
source_filename: cronometer-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: cronometer.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  7 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: cronometer.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"amazontrust.com\"\n  - 0 issuewild \"awstrust.com\"\n  - 0 issuewild \"godaddy.com\"\n  - 0 issuewild \"starfieldtech.com\"\n  - 0 iodef \"mailto:admin@cronometer.com\"\n  - 0 issuewild \"amazon.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/cronometer/security/cronometer-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Nutrition
- Health
- Fitness
- Calorie Counter
- Diet Tracking
- Mobile App
- Wellness
---
