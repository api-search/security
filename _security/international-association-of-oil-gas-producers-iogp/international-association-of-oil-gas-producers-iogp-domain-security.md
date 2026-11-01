---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: iogp.org
  spf: true
hosts:
- cert_expires: Nov 27 08:10:16 2026 GMT
  host: www.iogp.org
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: International Association Of Oil Gas Producers Iogp Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for International Association of Oil & Gas Producers (IOGP), probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: International Association of Oil & Gas Producers (IOGP)
provider_slug: international-association-of-oil-gas-producers-iogp
slug: international-association-of-oil-gas-producers-iogp-domain-security
source_filename: international-association-of-oil-gas-producers-iogp-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.iogp.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 27 08:10:16 2026 GMT\n  hsts: false\ndomains:\n- domain: iogp.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/international-association-of-oil-gas-producers-iogp/security/international-association-of-oil-gas-producers-iogp-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Energy
- Oil & Gas
- Non-profit
- Collaboration
---
