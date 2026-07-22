---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: artemishealth.com
  spf: true
hosts:
- cert_expires: Oct  3 17:12:12 2026 GMT
  host: www.artemishealth.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Artemis Health Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Artemis Health, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Artemis Health
provider_slug: artemis-health
slug: artemis-health-domain-security
source_filename: artemis-health-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.artemishealth.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 17:12:12 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: artemishealth.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/artemis-health/refs/heads/main/security/artemis-health-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Healthcare
- Analytics
- Health Data
- Employee Benefits
- Data Intelligence
- Health Plans
---
