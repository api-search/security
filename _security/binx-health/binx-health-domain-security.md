---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: mybinxhealth.com
  spf: true
hosts:
- cert_expires: Sep 27 13:08:32 2026 GMT
  host: mybinxhealth.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Binx Health Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Binx Health, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Binx Health
provider_slug: binx-health
slug: binx-health-domain-security
source_filename: binx-health-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-07'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: mybinxhealth.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 27 13:08:32 2026 GMT\n  hsts: false\ndomains:\n- domain: mybinxhealth.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/binx-health/refs/heads/main/security/binx-health-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Health
- Healthcare
- Diagnostics
- Molecular Diagnostics
- Point of Care Testing
- Medical Devices
- Sexual Health
- Laboratory
---
