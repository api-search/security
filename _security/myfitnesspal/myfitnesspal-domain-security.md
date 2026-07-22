---
api_specs:
- filename: myfitnesspal-notifications-asyncapi.yml
  format: yaml
  label: MyFitnessPal API v2
  slug: myfitnesspal-api-v2
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/myfitnesspal/refs/heads/main/asyncapi/myfitnesspal-notifications-asyncapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  - 0 issue "amazon.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: myfitnesspal.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: myfitnesspalapi.com
  spf: false
hosts:
- cert_expires: Sep 18 20:16:12 2026 GMT
  host: www.myfitnesspal.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 27 09:42:50 2026 GMT
  host: myfitnesspalapi.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 18 20:16:12 2026 GMT
  host: api.myfitnesspal.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Myfitnesspal Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for MyFitnessPal, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: MyFitnessPal
provider_slug: myfitnesspal
slug: myfitnesspal-domain-security
source_filename: myfitnesspal-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.myfitnesspal.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 18 20:16:12 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: myfitnesspalapi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 27 09:42:50 2026 GMT\n  hsts: false\n- host: api.myfitnesspal.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 18 20:16:12 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: myfitnesspal.com\n  dnssec: true\n  caa:\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: myfitnesspalapi.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/myfitnesspal/refs/heads/main/security/myfitnesspal-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Consumer
- Health and Fitness
- Nutrition
- Fitness Tracking
- Food Diary
- Wellness
- Webhooks
- OAuth
---
