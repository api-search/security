---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: seaporttx.com
  spf: true
hosts:
- cert_expires: Nov 22 19:32:46 2026 GMT
  host: seaporttx.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Seaport Therapeutics Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Seaport Therapeutics, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Seaport Therapeutics
provider_slug: seaport-therapeutics
slug: seaport-therapeutics-domain-security
source_filename: seaport-therapeutics-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: seaporttx.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 22 19:32:46 2026 GMT\n  hsts: false\ndomains:\n- domain: seaporttx.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/seaport-therapeutics/refs/heads/main/security/seaport-therapeutics-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Biotechnology
- Pharmaceuticals
- Life Sciences
- Clinical Trials
- Neuroscience
- Drug Delivery
---
