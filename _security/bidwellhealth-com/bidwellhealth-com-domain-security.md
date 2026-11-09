---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: bidwellhealth.com
  spf: true
hosts:
- cert_expires: Jan 11 15:46:42 2027 GMT
  host: bidwellhealth.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Bidwellhealth Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Bidwell Health, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Bidwell Health
provider_slug: bidwellhealth-com
slug: bidwellhealth-com-domain-security
source_filename: bidwellhealth-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: bidwellhealth.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 11 15:46:42 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: bidwellhealth.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/bidwellhealth-com/security/bidwellhealth-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Telehealth
- Healthcare
- Online Visits
- Cash Pay
- US
---
