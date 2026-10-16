---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: curbstand.com
  spf: true
hosts:
- cert_expires: Dec 30 13:17:55 2026 GMT
  host: curbstand.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Curbstand Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for CurbStand, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: CurbStand
provider_slug: curbstand
slug: curbstand-domain-security
source_filename: curbstand-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: curbstand.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 30 13:17:55 2026 GMT\n  hsts: false\ndomains:\n- domain: curbstand.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/curbstand/refs/heads/main/security/curbstand-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Valet
- Parking
- CarWash
- LosAngeles
---
