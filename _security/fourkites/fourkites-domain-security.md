---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: fourkites.com
  spf: true
hosts:
- cert_expires: Sep 14 19:00:47 2026 GMT
  host: www.fourkites.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- host: developers.fourkites.com
  https: false
- cert_expires: Nov 21 14:05:51 2026 GMT
  host: tracking-api.fourkites.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Fourkites Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for FourKites, probed live across 3 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: FourKites
provider_slug: fourkites
slug: fourkites-domain-security
source_filename: fourkites-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.fourkites.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 19:00:47 2026 GMT\n  hsts: false\n- host: developers.fourkites.com\n  https: false\n- host: tracking-api.fourkites.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 21 14:05:51 2026 GMT\n  hsts: null\ndomains:\n- domain: fourkites.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fourkites/refs/heads/main/security/fourkites-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Logistics
- Supply Chain Visibility
- Tracking
- Freight
- ETA
---
