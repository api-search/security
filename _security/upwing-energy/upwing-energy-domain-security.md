---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: upwingenergy.com
  spf: true
hosts:
- cert_expires: Nov 18 17:55:29 2026 GMT
  host: www.upwingenergy.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Upwing Energy Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Upwing Energy, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Upwing Energy
provider_slug: upwing-energy
slug: upwing-energy-domain-security
source_filename: upwing-energy-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.upwingenergy.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 18 17:55:29 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: upwingenergy.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/upwing-energy/refs/heads/main/security/upwing-energy-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Energy
- Oil and Gas
- Natural Gas
- Artificial Lift
- Gas Compression
- Industrial Hardware
- Manufacturing
- Turbomachinery
- Field Services
---
