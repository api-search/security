---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: waltzhealth.com
  spf: true
hosts:
- cert_expires: Oct 15 14:20:20 2026 GMT
  host: waltzhealth.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Waltz Health Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Waltz Health, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Waltz Health
provider_slug: waltz-health
slug: waltz-health-domain-security
source_filename: waltz-health-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: waltzhealth.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 15 14:20:20 2026 GMT\n  hsts: false\ndomains:\n- domain: waltzhealth.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/waltz-health/refs/heads/main/security/waltz-health-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Life Sciences
- Healthcare
- Pharmacy
- Drug Pricing
- Prescriptions
- Health Tech
- Pharmacy Benefits
- Marketplace
---
