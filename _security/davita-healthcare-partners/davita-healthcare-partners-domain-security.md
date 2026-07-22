---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: davita.com
  spf: true
hosts:
- cert_expires: Jul 31 03:30:08 2026 GMT
  host: www.davita.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Davita Healthcare Partners Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for DaVita HealthCare Partners, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: DaVita HealthCare Partners
provider_slug: davita-healthcare-partners
slug: davita-healthcare-partners-domain-security
source_filename: davita-healthcare-partners-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.davita.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jul 31 03:30:08 2026 GMT\n  hsts: false\ndomains:\n- domain: davita.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/davita-healthcare-partners/refs/heads/main/security/davita-healthcare-partners-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Coordinated Care
- Dialysis
- Healthcare
- Kidney Care
- Medicare Advantage
- Physician Group
---
