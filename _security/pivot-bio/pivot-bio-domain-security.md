---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: pivotbio.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: site.com
  spf: true
hosts:
- cert_expires: Oct  2 02:37:54 2026 GMT
  host: www.pivotbio.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 11 20:39:33 2026 GMT
  host: pivot-bio.my.site.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Pivot Bio Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Pivot Bio, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Pivot Bio
provider_slug: pivot-bio
slug: pivot-bio-domain-security
source_filename: pivot-bio-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.pivotbio.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 02:37:54 2026 GMT\n  hsts: false\n- host: pivot-bio.my.site.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 11 20:39:33 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: pivotbio.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: site.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pivot-bio/refs/heads/main/security/pivot-bio-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Agriculture
- AgTech
- Biotechnology
- Synthetic Biology
- Microbial Nitrogen
- Nitrogen Fixation
- Sustainable Agriculture
- Corn
- Wheat
- Sorghum
- Cotton
- Climate Tech
- Carbon Credits
---
