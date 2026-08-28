---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: powertapfuels.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: powertapcapital.com
  spf: true
hosts:
- cert_expires: Oct  6 17:36:58 2026 GMT
  host: www.powertapfuels.com
  hsts: false
  https: true
  tls_version: TLSv1.2
- cert_expires: Oct 25 13:00:57 2026 GMT
  host: powertapcapital.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Powertap Hydrogen Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for PowerTap Hydrogen, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: PowerTap Hydrogen
provider_slug: powertap-hydrogen
slug: powertap-hydrogen-domain-security
source_filename: powertap-hydrogen-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.powertapfuels.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct  6 17:36:58 2026 GMT\n  hsts: false\n- host: powertapcapital.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 25 13:00:57 2026 GMT\n  hsts: false\ndomains:\n- domain: powertapfuels.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n- domain: powertapcapital.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\nnote: 'Two corporate hosts: www.powertapfuels.com (operating company, Apache/static PHP) and powertapcapital.com\n  (public holding company, WordPress on LiteSpeed). Neither sets HSTS, neither domain has DNSSEC, CAA\n  or a DMARC record; both publish SPF. powertapcapital.com additionally serves a large volume of injected\n  third-party casino/gambling link spam in its rendered HTML (491 \"casino\"/\"slot\" occurrences in the homepage\n \
  \ body on 2026-08-26), which is a strong indicator of a compromised or SEO-injected WordPress install.'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/powertap-hydrogen/refs/heads/main/security/powertap-hydrogen-domain-security.yml
summary_line: TLSv1.2
tags:
- Company
- Energy
- Hydrogen
- Clean Energy
- Fueling Infrastructure
- Transportation
- Carbon Capture
- Heavy Duty Trucking
---
