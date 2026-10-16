---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: brilliantlightpower.com
  spf: true
hosts:
- cert_expires: Dec  3 04:27:38 2026 GMT
  host: brilliantlightpower.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Brilliant Light Power Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Brilliant Light Power, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Brilliant Light Power
provider_slug: brilliant-light-power
slug: brilliant-light-power-domain-security
source_filename: brilliant-light-power-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-06'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: brilliantlightpower.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  3 04:27:38 2026 GMT\n  hsts: false\ndomains:\n- domain: brilliantlightpower.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/brilliant-light-power/refs/heads/main/security/brilliant-light-power-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Energy
- Technology
- CleanEnergy
- Innovation
- Research
- Company
---
