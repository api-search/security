---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: iristelehealth.com
  spf: true
hosts:
- cert_expires: Oct  3 01:52:28 2026 GMT
  host: iristelehealth.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Iris Telehealth Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Iris Telehealth, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Iris Telehealth
provider_slug: iris-telehealth
slug: iris-telehealth-domain-security
source_filename: iris-telehealth-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-23'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: iristelehealth.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 01:52:28 2026 GMT\n  hsts: false\ndomains:\n- domain: iristelehealth.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/iris-telehealth/refs/heads/main/security/iris-telehealth-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Healthcare
- Telehealth
- Behavioral Health
- Mental Health
- Telepsychiatry
- Clinical Services
- Health Systems
- Artificial Intelligence
- Analytics
---
