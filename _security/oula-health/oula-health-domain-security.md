---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: oulahealth.com
  spf: true
hosts:
- cert_expires: Sep  8 21:02:15 2026 GMT
  host: oulahealth.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Oula Health Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Oula Health, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Oula Health
provider_slug: oula-health
slug: oula-health-domain-security
source_filename: oula-health-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: oulahealth.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  8 21:02:15 2026 GMT\n  hsts: false\ndomains:\n- domain: oulahealth.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/oula-health/refs/heads/main/security/oula-health-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Life Sciences
- Maternity Care
- Women's Health
- Healthcare Provider
- Pregnancy
- Digital Health
---
