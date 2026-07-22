---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: nozominetworks.com
  spf: true
hosts:
- cert_expires: Oct  1 15:27:17 2026 GMT
  host: www.nozominetworks.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Nozomi Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Nozomi, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Nozomi
provider_slug: nozomi
slug: nozomi-domain-security
source_filename: nozomi-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.nozominetworks.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 15:27:17 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: nozominetworks.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nozomi/refs/heads/main/security/nozomi-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Security
- OT Security
- IoT Security
- Industrial Control Systems
- Cybersecurity
- Critical Infrastructure
- Threat Detection
- Asset Visibility
- Operational Technology
---
