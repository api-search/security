---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: gigstamp.co.uk
  spf: true
hosts:
- cert_expires: Jan  1 23:59:59 2027 GMT
  host: gigstamp.co.uk
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: gigstamp Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for gigstamp, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: gigstamp
provider_slug: gigstamp-co-uk
slug: gigstamp-co-uk-domain-security
source_filename: gigstamp-co-uk-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-10'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: gigstamp.co.uk\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  1 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: gigstamp.co.uk\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/gigstamp-co-uk/security/gigstamp-co-uk-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Music
- Event
- United Kingdom
- Listings
- Community
- Company
---
