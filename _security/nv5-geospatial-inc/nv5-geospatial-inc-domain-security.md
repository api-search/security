---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: nv5.com
  spf: true
hosts:
- cert_expires: Dec 22 15:33:16 2026 GMT
  host: www.nv5.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Nv5 Geospatial Inc Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for NV5 Geospatial, Inc., probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: NV5 Geospatial, Inc.
provider_slug: nv5-geospatial-inc
slug: nv5-geospatial-inc-domain-security
source_filename: nv5-geospatial-inc-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.nv5.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 22 15:33:16 2026 GMT\n  hsts: false\ndomains:\n- domain: nv5.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/nv5-geospatial-inc/security/nv5-geospatial-inc-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Geospatial
- Engineering
- DataAnalytics
- Infrastructure
---
