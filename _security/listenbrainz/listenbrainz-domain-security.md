---
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: listenbrainz.org
  spf: true
hosts:
- host: listenbrainz.org
  https: false
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Listenbrainz Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ListenBrainz, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: ListenBrainz
provider_slug: listenbrainz
slug: listenbrainz-domain-security
source_filename: listenbrainz-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: listenbrainz.org\n  https: false\ndomains:\n- domain: listenbrainz.org\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/listenbrainz/security/listenbrainz-domain-security.yml
summary_line: DMARC
tags:
- Music
- OpenSource
- Community
- DataAPI
- Listening
---
