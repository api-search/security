---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: huddleupcare.com
  spf: true
hosts:
- cert_expires: Nov 25 07:31:37 2026 GMT
  host: www.huddleupcare.com
  hsts: true
  hsts_max_age: 31556952
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Dotcomtherapy Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Dotcomtherapy, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Dotcomtherapy
provider_slug: dotcomtherapy
slug: dotcomtherapy-domain-security
source_filename: dotcomtherapy-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-24'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.huddleupcare.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 25 07:31:37 2026 GMT\n  hsts: true\n  hsts_max_age: 31556952\ndomains:\n- domain: huddleupcare.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/dotcomtherapy/security/dotcomtherapy-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Education
- Healthcare
- Telehealth
- Therapy
---
