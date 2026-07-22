---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: cnx.com
  spf: true
hosts:
- cert_expires: Aug 22 21:01:35 2026 GMT
  host: www.cnx.com
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Cnx Resources Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for CNX Resources, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: CNX Resources
provider_slug: cnx-resources
slug: cnx-resources-domain-security
source_filename: cnx-resources-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.cnx.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Aug 22 21:01:35 2026 GMT\n  hsts: false\ndomains:\n- domain: cnx.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cnx-resources/refs/heads/main/security/cnx-resources-domain-security.yml
summary_line: TLSv1.2 · DMARC
tags:
- Energy
- Natural Gas
- Appalachia
- Upstream
- Oil and Gas
---
