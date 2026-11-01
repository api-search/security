---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: earthforce.io
  spf: true
hosts:
- cert_expires: Nov 24 20:53:39 2026 GMT
  host: www.earthforce.io
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Earth Force Technologies Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Earth Force Technologies, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Earth Force Technologies
provider_slug: earth-force-technologies
slug: earth-force-technologies-domain-security
source_filename: earth-force-technologies-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-24'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.earthforce.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 24 20:53:39 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: earthforce.io\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/earth-force-technologies/security/earth-force-technologies-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Forestry
- Environmental
- Technology
- Wildfire Prevention
---
