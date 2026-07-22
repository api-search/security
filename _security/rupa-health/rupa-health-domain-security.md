---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: rupahealth.com
  spf: true
hosts:
- cert_expires: Sep 18 21:49:15 2026 GMT
  host: www.rupahealth.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Rupa Health Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Rupa Health, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Rupa Health
provider_slug: rupa-health
slug: rupa-health-domain-security
source_filename: rupa-health-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.rupahealth.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 18 21:49:15 2026 GMT\n  hsts: false\ndomains:\n- domain: rupahealth.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rupa-health/refs/heads/main/security/rupa-health-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
- Healthcare
- Lab Testing
- Functional Medicine
- Diagnostics
- Health
- Practitioner Tools
---
