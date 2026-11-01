---
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  dmarc: false
  dnssec: false
  domain: owntracks.org
  spf: false
hosts:
- cert_expires: Nov 27 18:40:54 2026 GMT
  host: owntracks.org
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Owntracks Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for OwnTracks, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: OwnTracks
provider_slug: owntracks
slug: owntracks-domain-security
source_filename: owntracks-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: owntracks.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 27 18:40:54 2026 GMT\n  hsts: false\ndomains:\n- domain: owntracks.org\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/owntracks/security/owntracks-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- OpenSource
- LocationTracking
- Privacy
- MobileApps
---
