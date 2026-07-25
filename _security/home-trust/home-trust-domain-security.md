---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: hometrust.ca
  spf: true
hosts:
- cert_expires: Aug 30 23:59:59 2026 GMT
  host: www.hometrust.ca
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Home Trust Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Home Trust, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Home Trust
provider_slug: home-trust
slug: home-trust-domain-security
source_filename: home-trust-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-23'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.hometrust.ca\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 30 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: hometrust.ca\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/home-trust/refs/heads/main/security/home-trust-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Financial Services
- Banking
- Canada
- Trust Company
- Alternative Lending
- Mortgages
- Credit Cards
- Deposits
---
