---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: maribelhealth.com
  spf: true
hosts:
- cert_expires: Aug 23 05:42:03 2026 GMT
  host: www.maribelhealth.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Maribel Health Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Maribel Health, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Maribel Health
provider_slug: maribel-health
slug: maribel-health-domain-security
source_filename: maribel-health-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.maribelhealth.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 23 05:42:03 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: maribelhealth.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/maribel-health/refs/heads/main/security/maribel-health-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Healthcare
- Operational Intelligence
- Home Health
- Hospice
- Community Paramedicine
- Artificial Intelligence
- Care Coordination
- Health IT
---
