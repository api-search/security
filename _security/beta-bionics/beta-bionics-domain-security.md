---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: betabionics.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: betabionicsapi.com
  spf: true
hosts:
- cert_expires: Oct  6 05:44:56 2026 GMT
  host: www.betabionics.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.2
- cert_expires: Dec  1 23:59:59 2026 GMT
  host: portal.betabionics.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 10 23:59:59 2027 GMT
  host: us-main-prod.betabionicsapi.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Beta Bionics Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Beta Bionics, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Beta Bionics
provider_slug: beta-bionics
slug: beta-bionics-domain-security
source_filename: beta-bionics-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.betabionics.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct  6 05:44:56 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: portal.betabionics.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  1 23:59:59 2026 GMT\n  hsts: false\n- host: us-main-prod.betabionicsapi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 10 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: betabionics.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: betabionicsapi.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/beta-bionics/refs/heads/main/security/beta-bionics-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Company
- Health
- Healthcare
- Medical Devices
- Diabetes
- Automated Insulin Delivery
- Digital Health
- Remote Patient Monitoring
- HIPAA
- Connected Devices
---
