---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: ofgem.gov.uk
  spf: true
hosts:
- cert_expires: Dec  2 03:38:22 2026 GMT
  host: www.ofgem.gov.uk
  hsts: true
  hsts_max_age: 31557600
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Ofgem Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Ofgem, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Ofgem
provider_slug: ofgem
slug: ofgem-domain-security
source_filename: ofgem-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.ofgem.gov.uk\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  2 03:38:22 2026 GMT\n  hsts: true\n  hsts_max_age: 31557600\ndomains:\n- domain: ofgem.gov.uk\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ofgem/refs/heads/main/security/ofgem-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Energy
- United Kingdom
- Utilities
- Electricity
- Gas
- Energy Markets
- Regulator
- Smart Metering
- Open Data
- Energy Regulation
- Renewables
- Great Britain
---
