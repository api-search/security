---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: nekohealth.com
  spf: true
hosts:
- cert_expires: Sep 22 23:55:41 2026 GMT
  host: www.nekohealth.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Neko Health Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Neko Health, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Neko Health
provider_slug: neko-health
slug: neko-health-domain-security
source_filename: neko-health-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.nekohealth.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 22 23:55:41 2026 GMT\n  hsts: null\ndomains:\n- domain: nekohealth.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/neko-health/refs/heads/main/security/neko-health-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Health
- Healthcare
- Preventive Health
- Medical
- Body Scan
- Diagnostics
- Consumer Health
- OpenID Connect
---
