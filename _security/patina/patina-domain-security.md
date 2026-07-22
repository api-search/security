---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: patinahealth.com
  spf: true
hosts:
- cert_expires: Aug  6 07:27:40 2026 GMT
  host: patinahealth.com
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Patina Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Patina, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Patina
provider_slug: patina
slug: patina-domain-security
source_filename: patina-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: patinahealth.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Aug  6 07:27:40 2026 GMT\n  hsts: false\ndomains:\n- domain: patinahealth.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/patina/refs/heads/main/security/patina-domain-security.yml
summary_line: TLSv1.2 · DMARC
tags:
- Company
- Healthcare
- Primary Care
- Senior Care
- Telehealth
- Digital Health
- Closed
---
