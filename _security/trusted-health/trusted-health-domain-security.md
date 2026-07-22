---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: trustedhealth.com
  spf: true
hosts:
- cert_expires: Sep 25 21:26:17 2026 GMT
  host: trustedhealth.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Trusted Health Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Trusted Health, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Trusted Health
provider_slug: trusted-health
slug: trusted-health-domain-security
source_filename: trusted-health-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: trustedhealth.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 25 21:26:17 2026 GMT\n  hsts: false\ndomains:\n- domain: trustedhealth.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/trusted-health/refs/heads/main/security/trusted-health-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Marketplace
- Healthcare
- Nursing
- Staffing
- Travel Nursing
- Allied Health
- Workforce
---
