---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: characterbio.com
  spf: true
hosts:
- cert_expires: Nov 29 18:06:31 2026 GMT
  host: www.characterbio.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Character Biosciences Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Character Biosciences, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Character Biosciences
provider_slug: character-biosciences
slug: character-biosciences-domain-security
source_filename: character-biosciences-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-08'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.characterbio.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 29 18:06:31 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: characterbio.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/character-biosciences/refs/heads/main/security/character-biosciences-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Biotechnology
- Precision Medicine
- Genomics
- Therapeutics
- Startup
---
