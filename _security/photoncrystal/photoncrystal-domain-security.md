---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: photoncrystal.com
  spf: true
hosts:
- cert_expires: Jan 28 13:43:32 2027 GMT
  host: www.photoncrystal.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Photoncrystal Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Photon Crystal Energy, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Photon Crystal Energy
provider_slug: photoncrystal
slug: photoncrystal-domain-security
source_filename: photoncrystal-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.photoncrystal.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 28 13:43:32 2027 GMT\n  hsts: false\ndomains:\n- domain: photoncrystal.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/photoncrystal/refs/heads/main/security/photoncrystal-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Perovskite
- Photovoltaics
- Solar
- BIPV
- Clean Energy
- Manufacturing
- Hardware
---
