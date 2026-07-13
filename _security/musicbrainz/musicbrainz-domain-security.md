---
api_specs:
- filename: musicbrainz-web-service-openapi.yml
  format: yaml
  label: MusicBrainz Web Service v2
  slug: musicbrainz-web-service
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/musicbrainz/refs/heads/main/openapi/musicbrainz-web-service-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "digicert.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "comodoca.com"
  - 0 issue "sectigo.com"
  - 0 issuewild "digicert.com"
  - 0 issuewild "sectigo.com"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: musicbrainz.org
  spf: true
hosts:
- cert_expires: Oct 10 23:59:59 2026 GMT
  host: musicbrainz.org
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 10 23:59:59 2026 GMT
  host: beta.musicbrainz.org
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Musicbrainz Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for MusicBrainz, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: MusicBrainz
provider_slug: musicbrainz
slug: musicbrainz-domain-security
source_filename: musicbrainz-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: musicbrainz.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 10 23:59:59 2026 GMT\n  hsts: false\n- host: beta.musicbrainz.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 10 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: musicbrainz.org\n  dnssec: false\n  caa:\n  - 0 issue \"digicert.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"sectigo.com\"\n  - 0 issuewild \"digicert.com\"\n  - 0 issuewild \"sectigo.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/musicbrainz/refs/heads/main/security/musicbrainz-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Music
- Metadata
- Encyclopedia
- Open Data
- Catalog
- Identifiers
- ISRC
- ISWC
- MBID
- DiscID
- Artists
- Releases
- Recordings
- Works
- Labels
- Cover Art
- Open Source
- Non Profit
---
