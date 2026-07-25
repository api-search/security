---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: getmaple.ca
  spf: true
hosts:
- cert_expires: Oct 20 21:31:26 2026 GMT
  host: www.getmaple.ca
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Maple Health Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Maple, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Maple
provider_slug: maple-health
slug: maple-health-domain-security
source_filename: maple-health-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-24'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.getmaple.ca\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 20 21:31:26 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: getmaple.ca\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/maple-health/refs/heads/main/security/maple-health-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Healthcare
- Canada
- Telehealth
- Virtual Care
- Digital Health
- Mental Health
- e-Prescribing
- Remote Care
---
