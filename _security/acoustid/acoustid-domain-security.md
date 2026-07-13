---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: acoustid.org
  spf: true
hosts:
- cert_expires: Aug 20 08:30:52 2026 GMT
  host: acoustid.org
  hsts: true
  hsts_max_age: 15724800
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 20 08:30:52 2026 GMT
  host: api.acoustid.org
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Acoustid Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AcoustID, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: AcoustID
provider_slug: acoustid
slug: acoustid-domain-security
source_filename: acoustid-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: acoustid.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 20 08:30:52 2026 GMT\n  hsts: true\n  hsts_max_age: 15724800\n- host: api.acoustid.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 20 08:30:52 2026 GMT\n  hsts: null\ndomains:\n- domain: acoustid.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/acoustid/refs/heads/main/security/acoustid-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Audio
- Fingerprinting
- Music
- MusicBrainz
- Open Source
- Identification
---
