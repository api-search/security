---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: sarahealth.com
  spf: true
hosts:
- cert_expires: Oct 12 21:24:22 2026 GMT
  host: www.sarahealth.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Sara Health Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for SaRA Health, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: SaRA Health
provider_slug: sara-health
slug: sara-health-domain-security
source_filename: sara-health-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.sarahealth.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 12 21:24:22 2026 GMT\n  hsts: false\ndomains:\n- domain: sarahealth.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sara-health/refs/heads/main/security/sara-health-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Healthcare
- Digital Health
- Remote Therapeutic Monitoring
- Patient Engagement
- Physical Therapy
- SMS Messaging
- Medical Billing
---
