---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: ossiumhealth.com
  spf: true
hosts:
- cert_expires: Aug 21 12:48:43 2026 GMT
  host: ossiumhealth.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Ossium Health Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Ossium Health, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Ossium Health
provider_slug: ossium-health
slug: ossium-health-domain-security
source_filename: ossium-health-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ossiumhealth.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 21 12:48:43 2026 GMT\n  hsts: false\ndomains:\n- domain: ossiumhealth.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ossium-health/refs/heads/main/security/ossium-health-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Biotechnology
- Life Sciences
- Cell Therapy
- Regenerative Medicine
- Healthcare
- Bioengineering
---
