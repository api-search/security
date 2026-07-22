---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: quartethealth.com
  spf: true
hosts:
- cert_expires: Sep 15 11:11:43 2026 GMT
  host: www.quartethealth.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Quartet Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Quartet Health, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Quartet Health
provider_slug: quartet
slug: quartet-domain-security
source_filename: quartet-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.quartethealth.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 11:11:43 2026 GMT\n  hsts: false\ndomains:\n- domain: quartethealth.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/quartet/refs/heads/main/security/quartet-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Life Sciences
- Behavioral Health
- Mental Health
- Healthcare
- Care Coordination
- Value-Based Care
- Digital Health
---
