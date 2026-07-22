---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: workithealth.com
  spf: true
hosts:
- cert_expires: Sep 26 01:43:00 2026 GMT
  host: www.workithealth.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Workit Health Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Workit Health, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Workit Health
provider_slug: workit-health
slug: workit-health-domain-security
source_filename: workit-health-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.workithealth.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 26 01:43:00 2026 GMT\n  hsts: false\ndomains:\n- domain: workithealth.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/workit-health/refs/heads/main/security/workit-health-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
- Consumer
- Healthcare
- Telehealth
- Addiction Treatment
- Behavioral Health
- Digital Health
---
