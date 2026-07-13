---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: geogroup.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: bi.com
  spf: true
hosts:
- cert_expires: Aug 24 16:00:56 2026 GMT
  host: www.geogroup.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 20 07:40:55 2026 GMT
  host: bi.com
  hsts: true
  hsts_max_age: 0
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Geo Group Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for The GEO Group, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: The GEO Group
provider_slug: geo-group
slug: geo-group-domain-security
source_filename: geo-group-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.geogroup.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 24 16:00:56 2026 GMT\n  hsts: null\n- host: bi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 20 07:40:55 2026 GMT\n  hsts: true\n  hsts_max_age: 0\ndomains:\n- domain: geogroup.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: bi.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/geo-group/refs/heads/main/security/geo-group-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Corrections
- Private Prisons
- Immigration Detention
- Electronic Monitoring
- Surveillance
- Public Company
---
