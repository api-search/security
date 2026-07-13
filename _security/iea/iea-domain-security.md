---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: iea.org
  spf: true
hosts:
- cert_expires: Oct  3 21:59:40 2026 GMT
  host: www.iea.org
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 15 23:59:59 2027 GMT
  host: api.iea.org
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Iea Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for International Energy Agency (IEA), probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: International Energy Agency (IEA)
provider_slug: iea
slug: iea-domain-security
source_filename: iea-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.iea.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 21:59:40 2026 GMT\n  hsts: null\n- host: api.iea.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 15 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: iea.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/iea/refs/heads/main/security/iea-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Energy
- Electricity
- CO2
- Emissions
- Renewables
- Oil
- Statistics
- Climate
---
