---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: openchargemap.org
  spf: true
hosts:
- cert_expires: Jul 15 20:07:13 2026 GMT
  host: openchargemap.org
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Open Charge Map Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Open Charge Map, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Open Charge Map
provider_slug: open-charge-map
slug: open-charge-map-domain-security
source_filename: open-charge-map-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: openchargemap.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jul 15 20:07:13 2026 GMT\n  hsts: false\ndomains:\n- domain: openchargemap.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/open-charge-map/refs/heads/main/security/open-charge-map-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Transportation
- Public APIs
---
