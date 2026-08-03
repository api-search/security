---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: rzero.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: zendesk.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: coworkr.co
  spf: true
hosts:
- cert_expires: Sep 26 04:18:27 2026 GMT
  host: rzero.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 29 01:58:10 2026 GMT
  host: rzerosystems.zendesk.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 21 05:08:52 2026 GMT
  host: api.coworkr.co
  hsts: true
  hsts_max_age: 15768000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: R Zero Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for R-Zero, probed live across 3 host(s) and 3 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: R-Zero
provider_slug: r-zero
slug: r-zero-domain-security
source_filename: r-zero-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: rzero.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 26 04:18:27 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: rzerosystems.zendesk.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 01:58:10 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.coworkr.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 21 05:08:52 2026 GMT\n  hsts: true\n  hsts_max_age: 15768000\ndomains:\n- domain: rzero.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: zendesk.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: coworkr.co\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/r-zero/refs/heads/main/security/r-zero-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Smart Buildings
- Occupancy
- Sensors
- Internet of Things
- Indoor Air Quality
- Energy Efficiency
- HVAC
- Analytics
- Commercial Real Estate
- Workplace
---
