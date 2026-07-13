---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: addus.com
  spf: true
hosts:
- cert_expires: Sep 18 14:46:39 2026 GMT
  host: www.addus.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- host: developer.addus.com
  https: false
- host: api.addus.com
  https: false
kind: domain-security
layout: security
method: probed
name: Addus Homecare Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Addus HomeCare, probed live across 3 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Addus HomeCare
provider_slug: addus-homecare
slug: addus-homecare-domain-security
source_filename: addus-homecare-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.addus.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 18 14:46:39 2026 GMT\n  hsts: false\n- host: developer.addus.com\n  https: false\n- host: api.addus.com\n  https: false\ndomains:\n- domain: addus.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/addus-homecare/refs/heads/main/security/addus-homecare-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Home Care
- Healthcare Services
---
